# Quicklisp performance tests
In the following table one can find relative performance of clasp for some tasks:

Timings for version `"cclasp-boehm-0.4.2-3434-g3f70b6373-cst"`on `macosx 10.14.6 (mojave)` `CLASP_BUILD_MODE = 'faso'` `USE_COMPILE_FILE_PARALLEL=False`

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
* Remember that tests are done with default optimisation settings!

Benchmarked on: x86_64 Darwin Kernel Version 18.7.0: Fri Oct 30 12:37:06 PDT 2020; root:xnu-4903.278.44.0.2~1/RELEASE_X86_64 karsten-poecks-macbook-pro.local
|Benchmark|Best|Clozure Common Lisp Version 1.12 (v1.12-dev.3-125-g595a5cf4) DarwinX8664|ECL 20.4.24|SBCL 2.0.9.131-e70fbb9f9|clasp cclasp-boehm-0.4.2-3458-ga7a2855e3-cst|
| -- | -- | -- | -- | -- | -- |
|Date||20201121T0942|20201121T0938|20201121T0937|20201129T1008|
|COMPILER|      0.72|      0.82|      1.32|      0.72|     18.14|
|LOAD-FASL|      0.06|      0.11|      0.13|      0.06|      2.59|
|SUM-PERMUTATIONS|      0.20|      1.51|      2.07|      0.20|      2.59|
|WALK-LIST/SEQ|      0.01|      0.01|      0.01|      0.01|      0.02|
|WALK-LIST/MESS|      0.02|      0.02|      0.35|      0.02||
|BOYER|      0.17|      0.83|      0.63|      0.17|      1.03|
|BROWSE|      0.11|      0.30|      0.28|      0.11|      0.75|
|DDERIV|      0.11|      0.24|      0.57|      0.11|      2.00|
|DERIV|      0.11|      0.25|      0.64|      0.11|      2.20|
|DESTRUCTIVE|      0.09|      0.24|      0.41|      0.09|      0.63|
|DIV2-TEST-1|      0.18|      0.38|      0.73|      0.18|      2.10|
|DIV2-TEST-2|      0.25|      0.51|      1.04|      0.25|      2.44|
|FFT|      0.01|      0.06|      1.43|      0.01|      0.72|
|FRPOLY/FIXNUM|      0.13|      0.33|      1.08|      0.13|      0.83|
|FRPOLY/BIGNUM|      0.13|      0.51|      0.39|      0.13|      0.69|
|FRPOLY/FLOAT|      0.24|      0.57|      1.20|      0.24|      0.88|
|PUZZLE|      0.13|      0.42|      2.38|      0.13|      3.60|
|TAK|      0.09|      0.09|      0.86|      0.14|      0.97|
|CTAK|      0.21|      0.32|      1.24|      0.21||
|TRTAK|      0.07|      0.07|      0.86|      0.14|      0.98|
|TAKL|      0.25|      0.25|      0.66|      0.35|      0.61|
|STAK|      0.16|      0.51|      1.33|      0.16||
|FPRINT/UGLY|      0.39|      1.97|      0.95|      0.39|      3.25|
|FPRINT/PRETTY|      0.59|      2.03|      9.01|      0.59|     21.52|
|TRAVERSE|      0.54|      0.76|      1.87|      0.54|      3.04|
|TRIANGLE|      0.41|      0.56|      1.59|      0.41|      3.93|
|RICHARDS|      0.36|      0.87|      3.72|      0.36|      5.37|
|FACTORIAL|      0.07|      0.12|      0.14|      0.07|      0.39|
|FIB|      0.04|      0.04|      1.74|      0.11|      0.47|
|FIB-RATIO|      0.02|      0.03|      0.05|      0.02|      0.08|
|ACKERMANN|      0.64|      0.64|      3.85|      2.03|      7.57|
|MANDELBROT/COMPLEX|      0.15|      0.27|      0.21|      0.15|      2.43|
|MANDELBROT/DFLOAT|      0.01|      0.03|      0.74|      0.01|      2.26|
|MRG32K3A|      0.39|      4.11|      1.18|      0.39|      8.16|
|CRC40|      0.27|      1.20|      8.30|      0.27|      5.12|
|BIGNUM/ELEM-100-1000|      0.02|      0.56|      0.02|      0.04|      0.04|
|BIGNUM/ELEM-1000-100|      0.02|      3.33|      0.02|      0.06|      0.03|
|BIGNUM/ELEM-10000-1|      0.02|      3.52|      0.02|      0.03|      0.02|
|BIGNUM/PARI-100-10|      0.00|      0.34|      0.00|      0.01|      0.00|
|BIGNUM/PARI-200-5|      0.01|      9.56|      0.01|      0.02|      0.01|
|PI-DECIMAL/SMALL|      0.27|      1.23|      1.11|      0.27|      0.98|
|PI-DECIMAL/BIG|      0.12|      1.40|      0.75|      0.12|      0.65|
|PI-ATAN|      0.25|      1.33|      0.25|      0.44|      0.48|
|PI-RATIOS|      0.36|      3.68|      0.36|      0.58||
|HASH-STRINGS|      0.10|      2.64|      0.40|      0.10|      0.42|
|HASH-INTEGERS|      0.12|      1.25|      0.52|      0.12|      0.36|
|SLURP-LINES|      0.99|     10.83|      7.28|      0.99|     10.34|
|BOEHM-GC|      0.54|      4.95|      4.40|      0.54|     18.00|
|DEFLATE-FILE|      0.09|      0.16|      1.36|      0.09|      0.96|
|1D-ARRAYS|      0.02|      0.02|      0.16|      0.02|      0.21|
|2D-ARRAYS|      0.20|      0.66|      4.22|      0.20|      5.45|
|3D-ARRAYS|      0.48|      1.43|      9.05|      0.48|     11.02|
|BITVECTORS|      0.15|      0.27|      1.95|      0.17|      0.15|
|BENCH-STRINGS|      0.29|      0.79|      2.69|      0.88|      0.29|
|fill-strings/adjustable|      1.74|     11.97|      1.94|      1.74|      9.34|
|STRING-CONCAT|     15.43|     17.88|     25.19|     15.43|     45.00|
|SEARCH-SEQUENCE|      0.45|      1.22|      1.53|      0.45|      5.50|
|CLOS/defclass|      0.15|      0.18|      0.21|      0.15|      2.00|
|CLOS/defmethod|      0.10|      0.10|      0.18|      0.99|      4.15|
|CLOS/instantiate|      0.34|      2.09|      4.78|      0.34|      4.23|
|CLOS/simple-instantiate|      0.05|      3.69|     12.52|      0.05|      1.80|
|CLOS/methodcalls|      1.50|      1.50|      2.08|      2.70|      2.89|
|CLOS/method+after|      0.50|      0.94|      1.56|      0.50|     12.95|
|CLOS/complex-methods|      0.49|      0.54|      0.87|      0.49|      0.98|
|EQL-SPECIALIZED-FIB|      0.08|      0.36|      2.11|      0.08|     43.42|