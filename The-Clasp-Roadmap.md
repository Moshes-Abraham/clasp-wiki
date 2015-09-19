# In no particular order - except for the first two.

1. Speed - Clasp needs to be a performant language.  This means it needs to take more advantage of the inlining capabilities provided by Cleavir.
1. ANSI Common Lisp compliant - any differences between Clasp and the ANSI standard are bugs in Clasp.
1. Debugging - Clasp should expose the LLDB C++ API to Common Lisp and make the backtraces and stack frames available to SLDB for debugging.
1. Multithreading - Clasp needs threads.
1. Unicode - Clasp needs Unicode.
1. Unified Common Lisp code with ECL.
1. Rewrite the bclasp compiler so that it has an AST stage and a code generation stage - this will make it easy to identify at least some bindings that can go on the stack and should speed building clasp.
1. Improve the generic function dispatch in clasp.