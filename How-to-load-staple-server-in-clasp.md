You need same changes not yet in quicklisp, so
* Put the following in ~/quicklisp/local-projects/
  * bordeaux-threads (https://github.com/sionescu/bordeaux-threads.git , master). Does not seem to be updated in quicklisp, unless a new release of bordeaux-threads is made
  * usocket from https://github.com/usocket/usocket.git (pull request to integrate clasp has been merged)
  * plump from https://github.com/kpoeck/plump.git (works around a bug in clasp clos, see issue #698)
  * hunchentoot from https://github.com/kpoeck/hunchentoot.git

* To load:
```LISP
(load "~/quicklisp/setup.lisp")
(asdf:register-immutable-system :eclector)
(pushnew :hunchentoot-no-ssl *features*)
(ql:quickload "staple-server" :verbose t)
````


* To start (staple-server:start) 
* To stop (staple-server:stop) 