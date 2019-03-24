* clone clpython from https://github.com/kpoeck/cl-python.git (master) into ~/quicklisp/local-projects/fork-cl-python/
* (load "~/quicklisp/setup.lisp")
* (ql:quickload "clpython" :verbose t)
you will get the following error:
```lisp
Condition of type: SIMPLE-ERROR
Class #<The STANDARD-CLASS CLPYTHON::DICT-MIXIN> is not a valid superclass for #<The CLPYTHON::PY-META-TYPE CLPYTHON:PY-TYPE>
Available restarts:
(use :r1 to invoke restart 1)
````
* (load "~/quicklisp/local-projects/fork-cl-python/runtime/metaclass.lisp")
* :r1
* cl-python should be loaded
* test 
```lisp
COMMON-LISP-USER> (clpython:run "2 + 3")
5
COMMON-LISP-USER> (clpython:run "for i in range(4): print i")
0
1
2
3
NIL
````
* optionally (ASDF/OPERATE:TEST-SYSTEM "clpython") completes now having some tests disabled 
```lisp
End CLPython test
Errors detected in this test: 27 UNEXPECTED: 25
Successes this test:582
Return values of RUN-TESTS: (NIL 582 27 25)
````
