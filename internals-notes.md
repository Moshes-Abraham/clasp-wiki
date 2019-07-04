Return values
=============

NORMAL RETURNS
--------------

Basically, when returning unknown values (which is how it always is from functions, at present), we return a structure. This structure has one element that's a smart lispobj pointer (i.e., a T_sp) and one element that's a size_t. These are the primary return value and the number of return values (nret).

The primary return value is always set and valid. That is, if no values are returned, the primary is still NIL.

Additional return values are stored in the multiple value vector, which is a thread local C array plus a size_t count of return values. The primary return value and number of return values are not usually stored in this vector, but there is space for them and it's used for abnormal returns (below).

The return value structure is called `gctools::return_type` in C++, and is defined in core/lispCallingConvention.h. There is also an equivalent class, called `core::T_mv`, which is defined in gctools/multiple_value_pointers.h. It is used in C++, but somewhat sparingly - due to C++ weirdness it can't be returned in registers, so we don't use it.

If you're wondering why the gctools namespace thing is in the core directory, and the core namespace thing is in the gctools directory, I don't know either.

The multiple value vector structure is defined in core/MultipleValues.h.

SAVING VALUES
-------------

So far we have defined a single multiple values location. multiple-value-prog1 and its implicit users entail that we be able to temporarily save and restore multiple values. We do this by allocating a VLA of pointers and copying the multiple value vector into it. That is, basically

```
size_t nret = return_value.nret;
T_O* save[nret];
if (nret > 0) {
  save[0] = return_value.primary;
  for (size_t i = 1; i < nret; ++i) save[i] = mv[i];
}
...code...
for (size_t i = 1; i < nret; ++i) mv[i] = save[i];
return_value.primary = save[0];
return_value.nret = nret;
```

In some situations we want to save `mv[0]` as well. It should be obvious how that's accomplished.

In cclasp these are c`lasp-cleavir-hir:save-values-instruction` and `:load-values-instruction`. For the loop they call intrinsics `cc_save_values` and `cc_load_values`, which in turn call functions in multiple_value_pointers.h.

ABNORMAL RETURNS
----------------

When abnormally returning from a function, i.e. `cl:return-from`, we store the primary value and nret into the multiple value array as well before throwing the C++ exception.

Any unwind-protects encountered while unwinding save the entire multiple value vector as above for the duration of executing the cleanup.

The destination finally loads the number of return values and the primary value from the multiple value vector.
