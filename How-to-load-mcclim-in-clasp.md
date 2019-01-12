### Prerequisites
* clasp from dev as of 2019-01-12
* Put the following in ~/quicklisp/local-projects/
  * bordeaux-threads (https://github.com/sionescu/bordeaux-threads.git , master)  
  * clx (https://github.com/sharplispers/clx.git, master)
  * mcclim (https://github.com/McCLIM/McCLIM.git, master)

### To compile & load (takes 4 hours on my machine)
* (load "~/quicklisp/setup.lisp")
* (ql:quickload "clim-examples" :verbose t)
* (mcclim-truetype::autoconfigure-fonts)

### To test
* (clim-demo:demodemo) 
* or e.g. 
  * (clim:run-frame-top-level (clim:make-application-frame 'clim-demo::logic-cube))
  * (clim:run-frame-top-level (clim:make-application-frame 'calculator-demo::calculator-app))
  * (clim:run-frame-top-level (clim:make-application-frame 'clim-demo::address-book))
