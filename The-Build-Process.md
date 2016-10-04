# Bootstrap Stages
  1. `aclasp` is a CL interpreter written in C++ that loads a minimal CL system
  2. `bclasp` is a CLOS capable CL system, good enough to run [Cleavir](http://metamodular.com/cleavir.pdf)
  3. `cclasp` is created by loading Cleavir into `bclasp` and recompiling everything
