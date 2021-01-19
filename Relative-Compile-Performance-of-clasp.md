# Quicklisp performance tests
In the following table one can find relative performance of clasp for some tasks:

Timings for version `"cclasp-boehm-0.4.2-3434-g3f70b6373-cst"`on `macosx 10.14.6 (mojave)` `CLASP_BUILD_MODE = <default>` `USE_COMPILE_FILE_PARALLEL=<default>`

| Compile Task (real)| clasp(s) | ccl(s) | ecl(s) | sbcl(s) | factor clasp/sbcl | factor clasp/ecl |factor ecl/sbcl |
| ------------------ | -------- | ------ | -------| --------| ----------------- | ---------------- | ---------------| 
| cl-bench compiler|18.141|0.820|1.320|0.72|25.20|13.74|22.12|
| asdf |66.119|5.302|20.121|5.31|12.46|3.29|12.47|
| cl-jpeg  |27.875|1.127|139.247|1.46|19.07|0.20|24.73|
| ironclad |359.528|26.820|447.353|50.98|7.05|0.80|13.41|
| clx  |373.247|9.717|186.107|13.26|28.15|2.01|38.41|
| mcclim|1433.720|57.449|59.703|65.64|21.84|2.56|24.96|

Note that e.g. :mcclim depends on :clx and :cl-jpeg, so that order of timings is important

Commands used (fresh start after each compile in this order):
* `(time (compile-file "source-dir:src;lisp;modules;asdf;build;asdf.lisp"))`
* `(time (ql:quickload :cl-jpeg))`
* `(time (ql:quickload :ironclad))`
* `(time (ql:quickload :clx))`
* `(time (ql:quickload :mcclim))` and this include lots of other asdf systems

# Cl-Bench tests
To reproduce:

* Sources in https://gitlab.common-lisp.net/kpoeck/cl-bench.git, branch feature-clasp-clbench
* Execute `(load "load-cl-bench.lisp")`
* Remember that tests are done with default optimization settings!

Benchmarked on: x86_64 Darwin Kernel Version 18.7.0: Tue Nov 10 00:07:31 PST 2020; root:xnu-4903.278.51~1/RELEASE_X86_64 karsten-poecks-macbook-pro.local
|Benchmark|Best|Clozure Common Lisp Version 1.12 (v1.12-dev.3-125-g595a5cf4) DarwinX8664|ECL 20.4.24-develop|SBCL 2.0.11|clasp cclasp-boehm-0.4.2-3458-ga7a2855e3-cst|clasp cclasp-boehm-0.4.2-3593a-gcf622f75c-cst|clasp cclasp-boehm-0.4.2-3630-ge045444b6-cst-a|
| -- | -- | -- | -- | -- | -- | -- | -- |
|Date||20201121T0942|20201230T0742|20201227T0956|20201129T1008|20201227T1609|20210119T2209|
|COMPILER|      0,76|      0,82|      1,54|      0,76|     18,14|     15,43|     14,11|
|LOAD-FASL|      0,07|      0,11|      0,14|      0,07|      2,59|      2,36|      2,55|
|SUM-PERMUTATIONS|      0,21|      1,51|      2,12|      0,21|      2,59|      2,51|      3,10|
|WALK-LIST/SEQ|      0,01|      0,01|      0,01|      0,01|      0,02|      0,02|      0,02|
|WALK-LIST/MESS|      0,02|      0,02|      0,35|      0,02||||
|BOYER|      0,19|      0,83|      0,63|      0,19|      1,03|      0,96|      1,00|
|BROWSE|      0,11|      0,30|      0,26|      0,11|      0,75|      0,49|      0,49|
|DDERIV|      0,11|      0,24|      0,59|      0,11|      2,00|      1,82|      1,86|
|DERIV|      0,12|      0,25|      0,61|      0,12|      2,20|      2,02|      2,07|
|DESTRUCTIVE|      0,10|      0,24|      0,41|      0,10|      0,63|      0,61|      0,61|
|DIV2-TEST-1|      0,18|      0,38|      0,75|      0,18|      2,10|      2,07|      2,07|
|DIV2-TEST-2|      0,25|      0,51|      1,05|      0,25|      2,44|      2,51|      2,40|
|FFT|      0,02|      0,06|      1,53|      0,02|      0,72|      0,69|      0,72|
|FRPOLY/FIXNUM|      0,14|      0,33|      1,20|      0,14|      0,83|      0,80|      0,82|
|FRPOLY/BIGNUM|      0,13|      0,51|      0,41|      0,13|      0,69|      0,68|      0,76|
|FRPOLY/FLOAT|      0,25|      0,57|      1,28|      0,25|      0,88|      0,83|      0,84|
|PUZZLE|      0,16|      0,42|      2,63|      0,16|      3,60|      3,85|      3,50|
|TAK|      0,09|      0,09|      0,93|      0,14|      0,97|      1,13|      0,93|
|CTAK|      0,21|      0,32|      1,43|      0,21||||
|TRTAK|      0,07|      0,07|      0,89|      0,14|      0,98|      0,92|      0,93|
|TAKL|      0,25|      0,25|      0,70|      0,35|      0,61|      0,51|      0,42|
|STAK|      0,17|      0,51|      1,47|      0,17||||
|FPRINT/UGLY|      0,38|      1,97|      0,90|      0,38|      3,25|      2,85|      2,90|
|FPRINT/PRETTY|      0,61|      2,03|     10,15|      0,61|     21,52|     21,17|     19,73|
|TRAVERSE|      0,59|      0,76|      2,04|      0,59|      3,04|      2,86|      2,70|
|TRIANGLE|      0,42|      0,56|      1,77|      0,42|      3,93|      3,45|      3,70|
|RICHARDS|      0,37|      0,87|      4,06|      0,37|      5,37|      5,03|      5,21|
|FACTORIAL|      0,07|      0,12|      0,13|      0,07|      0,39|      0,40|      0,41|
|FIB|      0,04|      0,04|      1,84|      0,11|      0,47|      0,48|      0,45|
|FIB-RATIO|      0,02|      0,03|      0,05|      0,02|      0,08|      0,07|      0,07|
|ACKERMANN|      0,64|      0,64|      4,25|      2,12|      7,57|      7,68|      7,13|
|MANDELBROT/COMPLEX|      0,15|      0,27|      0,22|      0,15|      2,43|      2,49|      2,53|
|MANDELBROT/DFLOAT|      0,00|      0,03|      0,81|      0,00|      2,26|      2,39|      2,11|
|MRG32K3A|      0,39|      4,11|      1,30|      0,39|      8,16|      8,87|      7,76|
|CRC40|      0,28|      1,20|      8,61|      0,28|      5,12|      5,49|      5,18|
|BIGNUM/ELEM-100-1000|      0,03|      0,56|      0,03|      0,03|      0,04|      0,03|      0,04|
|BIGNUM/ELEM-1000-100|      0,02|      3,33|      0,02|      0,05|      0,03|      0,02|      0,02|
|BIGNUM/ELEM-10000-1|      0,02|      3,52|      0,02|      0,03|      0,02|      0,02|      0,02|
|BIGNUM/PARI-100-10|      0,00|      0,34|      0,00|      0,01|      0,00|      0,00|      0,00|
|BIGNUM/PARI-200-5|      0,01|      9,56|      0,01|      0,02|      0,01|      0,01|      0,01|
|PI-DECIMAL/SMALL|      0,28|      1,23|      1,18|      0,28|      0,98|      1,02|      0,96|
|PI-DECIMAL/BIG|      0,13|      1,40|      0,79|      0,13|      0,65|      0,73|      0,67|
|PI-ATAN|      0,27|      1,33|      0,27|      0,45|      0,48|      0,62|      0,51|
|PI-RATIOS|      0,40|      3,68|      0,40|      0,60||||
|HASH-STRINGS|      0,10|      2,64|      0,44|      0,10|      0,42|      0,48|      0,43|
|HASH-INTEGERS|      0,12|      1,25|      0,57|      0,12|      0,36|      0,37|      0,33|
|SLURP-LINES|      1,00|     10,83|      8,00|      1,00|     10,34|     11,11|     10,64|
|BOEHM-GC|      0,56|      4,95|      3,89|      0,56|     18,00|     16,97|     16,93|
|DEFLATE-FILE|      0,08|      0,16|      1,59|      0,08|      0,96|      0,87|      0,87|
|1D-ARRAYS|      0,02|      0,02|      0,22|      0,02|      0,21|      0,19|      0,19|
|2D-ARRAYS|      0,20|      0,66|      4,53|      0,20|      5,45|      5,38|      5,45|
|3D-ARRAYS|      0,47|      1,43|      9,11|      0,47|     11,02|     11,39|     11,69|
|BITVECTORS|      0,14|      0,27|      1,95|      0,18|      0,15|      0,14|      0,15|
|BENCH-STRINGS|      0,28|      0,79|      2,72|      0,97|      0,29|      0,33|      0,28|
|fill-strings/adjustable|      1,90|     11,97|      1,95|      1,90|      9,34|      9,56|      8,99|
|STRING-CONCAT|     15,25|     17,88|     26,15|     15,25|     45,00|     44,44|     41,09|
|SEARCH-SEQUENCE|      0,48|      1,22|      2,08|      0,48|      5,50|      6,11|      5,70|
|CLOS/defclass|      0,17|      0,18|      0,25|      0,17|      2,00|      2,03|      1,78|
|CLOS/defmethod|      0,10|      0,10|      0,26|      0,92|      4,15|      3,72|      3,27|
|CLOS/instantiate|      0,36|      2,09|      5,00|      0,36|      4,23|      4,12|      3,92|
|CLOS/simple-instantiate|      0,05|      3,69|     13,64|      0,05|      1,80|      1,51|      1,93|
|CLOS/methodcalls|      1,50|      1,50|      2,12|      2,70|      2,89|      2,90|      3,12|
|CLOS/method+after|      0,53|      0,94|      1,65|      0,53|     12,95|      4,20|      3,83|
|CLOS/complex-methods|      0,41|      0,54|      0,78|      0,41|      0,98|      1,05|      0,94|
|EQL-SPECIALIZED-FIB|      0,07|      0,36|      2,08|      0,07|     43,42|      0,42|      0,42|