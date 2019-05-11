* clone clpython from https://github.com/kpoeck/cl-python.git (master) into ~/quicklisp/local-projects/fork-cl-python/
* (load "~/quicklisp/setup.lisp")
* (ql:quickload "clpython" :verbose t)

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
Errors detected in this test: 33 UNEXPECTED: 31
Successes this test:831

Return values of RUN-TESTS: (NIL 831 33 31)
Top level in: #<PROCESS TOP-LEVEL @0x11dbb4cd9>.
COMMON-LISP-USER> 
````
There are a lot of SyntaxErrors in ' (run-pretty-printer-test)' that I caught with (handler-case ..) since they caused the test to abort
