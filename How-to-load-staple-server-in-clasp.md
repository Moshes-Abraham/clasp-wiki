You need same changes not yet in quicklisp, so
* Put the following in ~/quicklisp/local-projects/
  * bordeaux-threads (https://github.com/sionescu/bordeaux-threads.git , master). Does not seem to be updated in quicklisp, unless a new release of bordeaux-threads is made
  * usocket from https://github.com/clasp-developers/usocket (pull request to uscoket has been made)
  * plump with the following change in dom.lisp
```lisp
(defgeneric serialize-object (node)
...
(:method ((nodes vector))
    (loop for child across nodes
       do (serialize child *stream*)))
  #+clasp
  (:method ((nodes array))
    ;;; better be one-dimensional
    (if (null (rest (array-dimensions nodes)))
        (loop for index from 0 to (length nodes)
           do (serialize (aref nodes index) *stream*))
        (warn "Multilevel-array in serialize-object ~a ~%" nodes)))
  #+clasp
  (:method ((nodes t))
    nil)
  )
````
*
  * hunchentoot-v1.2.38 with the following change in set-timeouts.lisp
```lisp
(defun set-timeouts (usocket read-timeout write-timeout)
#+:(or abcl clasp)
  (when write-timeout
    (warn "Unimplemented."))
  #-(or :clisp :allegro :openmcl :sbcl :lispworks :cmu :ecl :abcl :clasp)
  (not-implemented 'set-timeouts))
````

* To load:
  * (load "~/quicklisp/setup.lisp")
  * (asdf:register-immutable-system :eclector)
  * (ql:quickload "staple-server" :verbose t)
* To start (staple-server:start) 
* To stop (staple-server:stop) 