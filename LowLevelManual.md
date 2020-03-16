# Debugger

Debugging works within a dynamic environment with the following dynamic variables defined:
* `sys:*backtrace*` - A list of backtrace frames.
* `sys:*ihs-top*` - The index of the stack frame with the highest index.
* `sys:*ihs-base*` - The index of the stack frame with the lowest index. This is the most recent frame.
* `sys:*ihs-mode*` - The backtrace can display only lisp frames (set to `'sys:ihs-common-lisp`) or all frames (set to `sys:ihs-all`).
* `sys:*ihs-current*` - The index of the current frame.

Backtrace frames are simple structs of type `vector`, they are essentially defined using the following.  Read accessors are defined for all of the slots and write accessors for just a few of them.
```lisp
(defstruct (sys:backtrace-frame (:named) (:type vector))
  type return-address raw-name function-name print-name
  frame-size frame-offset function-start-address function-end-address
  base-pointer arguments closure function-description)
```

Convenience functions are defined for working with the backtrace:

* `sys:ihs-bounded (index)` - Returns index if index is a valid index into the backtrace otherwise if index is negative it returns 0 or too large it returns `(1- (length sys:*backtrace*))`
* `sys:ihs-backtrace-frame (index)` - Returns the frame at index.
* `sys:ihs-source-information (&optional (index sys:*ihs-current*))` - Return the source information for the frame at index as values: filename function-name source line column function-start-line discriminator
* `sys:ihs-return-address (&optional (index sys:*ihs-current*))` - Return a pointer containing the return address of this frame.

