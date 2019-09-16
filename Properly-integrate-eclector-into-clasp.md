To get libraries that modify the readtable to compile with clasps cst compiler, the following seem to work:
```lisp
(in-package :cl-user)

(setq eclector.readtable:*readtable* cl:*readtable*)

(defmethod eclector.readtable:syntax-type  ((readtable cl:readtable) char)
  (core:syntax-type readtable char))

(defmethod eclector.readtable:get-macro-character ((readtable cl:readtable) char)
  (cl:get-macro-character char readtable))

````