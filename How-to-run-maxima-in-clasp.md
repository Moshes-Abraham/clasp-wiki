* `git clone https://git.code.sf.net/u/kpoeck2018/maxima u-kpoeck2018-maxima` Original in https://sourceforge.net/p/maxima/code/ci/master/tree/
* `clasp`
* `(load "configure.lisp")`
* `(configure)`
* `(core:quit)`
* cd src/
* clasp
* `(load "maxima-build.lisp")`
* `(maxima-compile)`
* `(core:quit)`
* `clasp`
* `(load "maxima-build.lisp")`
* `(maxima-load)`
* `(cl-user::run)`
* To test, e.g. 
````
(%i1) integrate(x*sin(a*x),x);
                            sin(a x) - a x cos(a x)
(%o1)                       -----------------------
                                       2
                                      a
````
* Test suites
   * Standard `run_testsuite();` (I fixed a bug in clasp regarding log of big numbers. Might crash w/o the fix)
   * Extended `run_testsuite(share_tests='only);`
   * Both `run_testsuite(share_tests=true);` This takes 40GB and 2 hours on my machine
* to lisp `to_lisp();`
* To quit to os `quit();` 