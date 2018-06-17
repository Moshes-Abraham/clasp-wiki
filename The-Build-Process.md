# Bootstrap Stages

Until the two are merged, see also: [docs/bootstrap.rst](https://github.com/clasp-developers/clasp/blob/dev/docs/bootstrap.rst)

## `iclasp`
is an interpreter for a subset of CL written in C++.

iclasp is already capable of calling the LLVM functions (see the `llvm-sys` package).

iclasp expands macros repeatedly, every time they are reached. This makes it rather slow with `loop` and friends.

## `aclasp`
is iclasp after loading a minimal CL system that is capable of `compile-file`-ing a subset of CL.

`compile-file` happens by calling the LLVM machinery at runtime.

`./waf build_rboehm` starts iclasp and has it load the aclasp Common Lisp source code as interpreted code; i.e. absolutely no Common Lisp compilation happens up to this point.

At this point aclasp is used to compile itself (i.e. calling `compile-file` on the CL source files that are implementing aclasp), and when a file is compiled, it is loaded into the running image, which leads to a gradual speedup of this process of compilation.

`./waf build_aboehm` then links the `compile-file`'d code into a fasl called `aclasp-boehm-image.fasl`. Run `iclasp-boehm` with this image and you get what you get when you run `./waf build_rboehm`, but everything is compiled now (i.e. faster).

## `bclasp`
is a complete CL system that is now able to run [Cleavir](http://metamodular.com/cleavir.pdf), which is a modern full-blown CL compiler that requires full CL support to run, CLOS included.

## `cclasp`
is created by loading Cleavir into `bclasp` and recompiling everything.

# Building with extensions
## Requiremens for the build infrastructure

The build script of extensions must be able to do at least the following:
* register .cc/.h files for inclusion
* register .lisp files for inclusion
* register link artifacts for the linking of the final exe