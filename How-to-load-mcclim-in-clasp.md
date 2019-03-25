### Prerequisites
* clasp from dev as of 2019-01-12
* Put the following in ~/quicklisp/local-projects/
  * bordeaux-threads (https://github.com/sionescu/bordeaux-threads.git , master)  
  * clx (https://github.com/sharplispers/clx.git, master)
  * mcclim (https://github.com/McCLIM/McCLIM.git, master)

### To compile & load (takes 4 hours on my machine)
```common-lisp
(load "~/quicklisp/setup.lisp")
(ql:quickload "clim-examples" :verbose t)
(mcclim-truetype::autoconfigure-fonts)
````
### To test
* (clim-demo:demodemo) 
* or e.g. 
  * (clim:run-frame-top-level (clim:make-application-frame 'clim-demo::logic-cube))
  * (clim:run-frame-top-level (clim:make-application-frame 'calculator-demo::calculator-app))
  * (clim:run-frame-top-level (clim:make-application-frame 'clim-demo::address-book))
### IR Visualizer (cleavir-ir-visualizer)
* make the asd files known:
  * (asdf:load-asd (pathname "sys:kernel;contrib;sicl;Code;Cleavir;Intermediate-representation;Visualizer;cleavir-ir-visualizer.asd"))
  * (asdf:load-asd (pathname "sys:kernel;contrib;sicl;Code;Cleavir;Intermediate-representation;cleavir-ir.asd"))
  * (asdf:load-asd (pathname "sys:kernel;contrib;sicl;Code;Cleavir;Meter;cleavir-meter.asd"))
  * (asdf:load-asd (pathname "~/quicklisp/software/mcclim-git/Apps/Inspector/clouseau.asd")) adapt to your directory-structure
  * (asdf:load-asd (pathname "sys:kernel;contrib;sicl;Code;Cleavir;Intermediate-representation;Hir;cleavir-hir.asd"))
* (ql:quickload "cleavir-ir-visualizer" :verbose t)
* to test
```common-lisp
(cl:in-package #:cleavir-ir-visualizer)
(defvar *ast*)
(defvar *hir*)
(setq *ast* (cleavir-generate-ast:generate-ast '(lambda(a) (+ a 1)) clasp-cleavir:*clasp-env* clasp-cleavir:*clasp-system*))
(setq *hir* (cleavir-ast-to-hir:compile-toplevel-unhoisted *ast*))
(cleavir-ir-visualizer:visualize *hir*)
````
