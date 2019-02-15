You need same changes not yet in quicklisp, so
* Put the following in ~/quicklisp/local-projects/
  * bordeaux-threads (https://github.com/sionescu/bordeaux-threads.git , master). Does not seem to be updated in quicklisp, unless a new release of bordeaux-threads is made
  * usocket from https://github.com/clasp-developers/usocket (pull request to uscoket has been made)
  * plump from https://github.com/kpoeck/plump.git (works around a bug in clasp clos, see issue #698)
  * hunchentoot-v1.2.38 with the following change in set-timeouts.lisp
```lisp
(defun set-timeouts (usocket read-timeout write-timeout)
#+:(or abcl clasp)
  (when write-timeout
    (warn "Unimplemented."))
  #-(or :clisp :allegro :openmcl :sbcl :lispworks :cmu :ecl :abcl :clasp)
  (not-implemented 'set-timeouts))
```

* To load:
  * (load "~/quicklisp/setup.lisp")
  * (asdf:register-immutable-system :eclector)
  * (ql:quickload "staple-server" :verbose t)

```
* To start (staple-server:start) 
* To stop (staple-server:stop) 