* get newest clasp and build
* fork https://github.com/kpoeck/trial.git into ~/quicklisp/local-projects/
* fork https://github.com/kpoeck/3d-vectors.git in ~/quicklisp/local-projects/
* compile cl-jpeg with the serial compiler
```lisp
build/clasp
(load "~/quicklisp/setup.lisp")
(setq clasp-cleavir::*use-ast-interpreter* nil)
;;; be very patient, needs 1 hour on my machine
(ql:quickload :cl-jpeg)
````
* load trial
```lisp
build/clasp
;;; be very patient
(ql:quickload :cl-jpeg)
````
* try it out
```lisp
;;; I had to delete :trial from the dependencies in the following :asd, don't know yet whether this is a clasp error
(ql:quickload :trial-glfw :verbose t)
(trial:launch 'trial::workbench)
````