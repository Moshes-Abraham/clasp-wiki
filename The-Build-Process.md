# Bootstrap Stages
  1. `iclasp` is a CL interpreter written in C++
  2. `aclasp` is iclasp after loading a minimal CL system

  3. `bclasp` is a CLOS capable CL system, good enough to run [Cleavir](http://metamodular.com/cleavir.pdf)
  4. `cclasp` is created by loading Cleavir into `bclasp` and recompiling everything

# Building with extensions
## Requiremens for the build infrastructure

The build script of extensions must be able to do at least the following:
* register .cc/.h files for inclusion
* register .lisp files for inclusion
* register link artifacts for the linking of the final exe