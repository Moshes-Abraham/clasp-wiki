In the following table one can find relative performance of clasp for some tasks:

Timings for version `cclasp-boehm-0.4.2-2692-g00d68d383-cst`on `macosx 10.14.6 (mojave)` `CLASP_BUILD_MODE = 'faso'` `USE_COMPILE_FILE_PARALLEL=True`

| Compile Task (real)| clasp(s) | ecl(s) | sbcl(s) | factor clasp/sbcl | factor clasp/ecl |factor ecl/sbcl |
| ------------------ | -------- | ------ | ------- | ----------------- | ---------------- | -------------- | 
| cl-bench gabriel |35.0|6,170|0.711|49.23|5.67|8.68|
| asdf  |123.399|20.145|5.872|21.01|6.13|3.43|
| cl-jpeg |119.012|128.09|1.531|77.73|0.93|83.62|
| ironclad |5355.203|400.671|53.792|99.55|13.37|7.45| 
| clx |1241.959|187.031|14.933|83.17|6.61|12.52|
| mcclim |4366.509|error in cl-unicode|66.045|66.11|missing|missing|

Note that e.g. :mcclim depends on :clx and :cl-jpeg, so that order of timings is important

Commands used (in the same session in this order):
* `(time (compile-file "source-dir:src;lisp;modules;asdf;build;asdf.lisp"))`
* `(time (ql:quickload :cl-jpeg))`
* `(time (ql:quickload :ironclad))`
* `(time (ql:quickload :clx))`
* `(time (ql:quickload :mcclim))`