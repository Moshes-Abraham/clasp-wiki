Clasp startup has a problem in that when it starts up CLOS in boot.lsp, every class needs to be created and this invokes the compiler via EVAL.

This is the code that is slow:

    ;;;
    ;;; make-empty-standard-class compiles a lot of code using EVAL
    ;;;
    ;;; This is being run every time Clasp starts up!
    ;;; We have to figure out how ECL avoids this.
    ;;;
    (let* ((class-hierarchy '#.+class-hierarchy+))
      (let ((all-classes (loop for c in class-hierarchy
	   		    for class = (progn
				      (apply #'make-empty-standard-class c))
			    collect class)))
