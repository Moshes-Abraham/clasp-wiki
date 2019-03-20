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
* optionally (ASDF/OPERATE:TEST-SYSTEM "clpython")
* This errors pretty fast, but shows some passed tests
