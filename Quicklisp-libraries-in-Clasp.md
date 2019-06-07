In the following table one can find the state of popular quicklisp distributions in clasp.
Libraries selected according to http://blog.quicklisp.org/2018/03/download-stats-for-february-2018.html

| System | Compiles | Testsuite | Testresults | Tweaks |
| ----------------- | ------- | ---------------- | ---------------- |--------------- |
|(ql:quickload "alexandria" :verbose t)|Yes|(ql:quickload "alexandria-tests" :verbose t) (alexandria-tests::run-tests :compiled nil) (alexandria-tests::run-tests :compiled t)| 226 tests ok|circular-tree-p.2 crashes to the os| 
|(ql:quickload "closer-mop" :verbose t)|Yes|No tests available|||
|(ql:quickload "babel" :verbose t)|Yes|(ql:quickload "babel-tests")(babel-tests:run)| #<test-run: 56 tests, 473 assertions, 0 failures in 52.81187 sec>|Needs to fix the tests so that "?" is not a string of base-char (might be a clasp bug, not sure)|
|(ql:quickload "cl-ppcre" :verbose t)|Yes|(ql:quickload :cl-ppcre-test) (cl-ppcre-test::run-all-tests)|Some tests failed. (probably 1||
|(ql:quickload "split-sequence" :verbose t)|Yes|(ql:quickload :split-sequence/tests) (split-sequence/tests::run! :split-sequence)| Pass: 60 (100%)||
|(ql:quickload "trivial-features" :verbose t)|Yes|(ql:quickload :trivial-features-tests) (trivial-features-tests::do-tests)|No tests failed.||
|(ql:quickload "iterate" :verbose t)|Yes|(ql:quickload :iterate/tests) (REGRESSION-TEST:do-tests)| 9 out of 268 total tests failed:||
|(ql:quickload "trivial-gray-streams" :verbose t)|Yes|(ql:quickload :trivial-gray-streams-test) (trivial-gray-streams-test::run-tests)|4 failed tests||
|(ql:quickload "bordeaux-threads" :verbose t)|Yes|(ql:quickload :bordeaux-threads/test)(bordeaux-threads/test::run! :bordeaux-threads)| Did 25 checks Pass: 23 (92%) Skip: 0 ( 0%) Fail: 2 ( 8%)|Need (https://github.com/sionescu/bordeaux-threads.git , master).|
|(ql:quickload "anaphora" :verbose t)|Yes|(ql:quickload :anaphora/test :verbose t)(rt:do-tests)|No tests failed.||
|(ql:quickload "let-plus" :verbose t)|Yes|(ql:quickload :let-plus/tests)(let-plus-tests::run)|#<Results for LET-PLUS-TESTS [24 Successful tests]>|requires lift fix, see above|
|(ql:quickload "cffi" :verbose t)|Yes|(ql:quickload "cffi-tests" :verbose t) (cffi-tests::run-all-cffi-tests)|16 out of 323 total tests failed: (interpreted) EXC_BAD_ACCESS with compiled tests in SUMPAIR^CFFI-TEST||
|(ql:quickload "trivial-garbage" :verbose t)|Yes||||
|(ql:quickload "flexi-streams" :verbose t)|Yes||||
|(ql:quickload "nibbles" :verbose t)|Yes|||`(setq cmp::*compile-file-parallel* nil)`|
|(ql:quickload "puri" :verbose t)|Yes||||
|(ql:quickload "usocket" :verbose t)|Yes||||
|(ql:quickload "trivial-backtrace" :verbose t)|Yes|||
|(ql:quickload "more-conditions" :verbose t)|Yes||||
|(ql:quickload "chunga" :verbose t)|Yes||||
|(ql:quickload "cl-fad" :verbose t)|Yes||||
|(ql:quickload "cl+ssl" :verbose t)|Yes||||
|(ql:quickload "cl-base64" :verbose t)|Yes||||
|(ql:quickload "esrap" :verbose t)|Yes||||
|(ql:quickload "chipz" :verbose t)|Yes||||
|(ql:quickload "named-readtables" :verbose t)|Yes||||
|(ql:quickload "drakma" :verbose t)|Yes||||
|(ql:quickload "local-time" :verbose t)|Yes||||
|(ql:quickload "ironclad" :verbose t)|Compiling forever|||export GC_INITIAL_HEAP_SIZE=40G|
|(ql:quickload "parse-number" :verbose t)|Yes||||
|(ql:quickload "fiveam" :verbose t)|Yes||||
|(ql:quickload "closure-common" :verbose t)|Yes||||
|(ql:quickload "cxml" :verbose t)|Yes||||
|(ql:quickload "log4cl" :verbose t)|No|||Condition of type: PATTERN-LAYOUT-ERROR|
|(ql:quickload "optima" :verbose t)|Yes||||
|(ql:quickload "parser.common-rules" :verbose t)|Yes||||
|(ql:quickload "cl-unicode" :verbose t)|Yes||||
|(ql:quickload "cl-interpol" :verbose t)|Yes||||
|(ql:quickload :lparallel-test) |Yes|(lparallel-test:execute)| -> Success: 171 tests, 119190 checks.||
|(ql:quickload "lift" :verbose t)|Yes|(ql:quickload :lift-test)(lift:run-tests :suite 'lift-test::lift-test)|#<Results for LIFT-TEST 107 Tests, 2 Failures>|use version from https://github.com/gwkkwg/lift.git|
|(ql:quickload "cl-dot" :verbose t)|Yes||||
|(ql:quickload "cl-syntax" :verbose t)|Yes||||
|(ql:quickload "cl-annot" :verbose t)|Yes||||
|(ql:quickload "cxml-stp" :verbose t)|No|||XPATH: Condition of type: PPCRE-SYNTAX-ERROR |
|(ql:quickload "cl-store" :verbose t)|Yes|(oos 'load-op :cl-store-tests)|6 out of 114 total tests failed: CIRC.5, CIRC.6, CIRC.9, CIRC.12, CIRC.13, CORRECT.LIST.1.|CIRC.16 fails in printing, Use https://github.com/kpoeck/cl-store.git|
|(ql:quickload "fare-utils" :verbose t)|Yes||||
|(ql:quickload "fare-quasiquote" :verbose t)|Yes||||
|(ql:quickload "xml.location" :verbose t)|No|||XPATH: Condition of type: PPCRE-SYNTAX-ERROR |
|(ql:quickload "cl-utilities" :verbose t)|Yes||||
|(ql:quickload "utilities.print-tree" :verbose t)|No|||Error in clasp, unicode strings don't survive compile-file, see https://github.com/clasp-developers/clasp/issues/723|
|(ql:quickload "trivial-utf-8" :verbose t)|Yes||||
|(ql:quickload :static-vectors :verbose t)|Yes|(ql:quickload :static-vectors/test :verbose t) (5am:run! :static-vectors)| Did 24 checks. Pass: 22 (91%) Skip: 0 ( 0%) Fail: 2 ( 8%)|Version from https://github.com/sionescu/static-vectors.git|
|(ql:quickload "fare-mop" :verbose t)|Yes||||
|(ql:quickload "inferior-shell" :verbose t)|Yes|(ql:quickload "inferior-shell/test") (inferior-shell-test::test-suite)|#<test-run: 2 tests, 1 assertion, 1 failure in 24.73289 sec (0 failed assertions, 1 error, none expected)>|Need to define #\cr|  
|(ql:quickload "quri" :verbose t)|Yes||||
|(ql:quickload "metabang-bind" :verbose t)|Yes||||
|(ql:quickload "trivial-indent" :verbose t)|Yes||||
|(ql:quickload "md5" :verbose t)|Yes||||
|(ql:quickload "documentation-utils" :verbose t)|Yes||||
|(ql:quickload "fast-io" :verbose t)|Yes||||
|(ql:quickload "uuid" :verbose t)|No|||ironclad|
|(ql:quickload "array-utils" :verbose t)|Yes||||
|(ql:quickload "plump" :verbose t)|Yes||||
|(ql:quickload "djula" :verbose t)|No||||
|(ql:quickload "symbol-munger" :verbose t)|Yes||||
|(ql:quickload "cl-slice" :verbose t)|Yes||||
|(ql:quickload "collectors" :verbose t)|Yes||||
|(ql:quickload "gettext" :verbose t)|Yes||||
|(ql:quickload "arnesi" :verbose t)|Yes||||
|(ql:quickload "hunchentoot" :verbose t)|Yes||||
|(ql:quickload "access" :verbose t)|Yes||||
|(ql:quickload "cl-locale" :verbose t)|No||||
|(ql:quickload "simple-date-time" :verbose t)|Yes||||
|(ql:quickload "ieee-floats" :verbose t)|Yes||||
|(ql:quickload "prove" :verbose t)|Yes||||
|(ql:quickload "yason" :verbose t)|No|||Condition of type: MALFORMED-LAMBDA-LIST-PATTERN|
|(ql:quickload "asdf-system-connections" :verbose t)|Yes||||
|(ql:quickload "metatilities-base" :verbose t)|Yes|`(ql:quickload "metatilities-base-test" :verbose t)(let ((LIFT:*CURRENT-ASDF-SYSTEM-NAME* (asdf:find-system "metatilities-base-test")))(lift:run-tests :config :generic))`|Test Report for /Users/karstenpoeck/quicklisp/local-projects/fork-metatilities-base/lift-standard.config: 9 tests run, all passed!||
|(ql:quickload "cl-containers" :verbose t)|Yes|`(ql:quickload "cl-containers-test" :verbose t)(let ((LIFT:*CURRENT-ASDF-SYSTEM-NAME* (asdf:find-system "cl-containers-test")))(lift:run-tests :config :generic))`|Test Report for /Users/karstenpoeck/quicklisp/dists/quicklisp/software/cl-containers-20170403-git/lift-standard.config: 9 tests run, all passed!||
|(ql:quickload "rfc2388" :verbose t)|Yes||||
|(ql:quickload "postmodern" :verbose t)|Changes needed|(ql:quickload "postmodern/tests" :verbose t) (cl-postgres-tests::prompt-connection) (fiveam::run! :postmodern) And you need a database| Did 317 checks. Pass: 314 (99%) Skip: 0 ( 0%) Fail: 3 ( 0%)|in postmodern.asd add #clasp to the eval-when. Error in query.lisp, where (defvar *class-finalize-lock* (bt:make-lock)) is not preceeded by #+:postmodern-thread-safe|
|(ql:quickload "fast-http" :verbose t)|No thread #1, queue = 'com.apple.main-thread', stop reason = signal SIGSTOP ||||
|(ql:quickload "trivial-mimes" :verbose t)|Yes||||
|(ql:quickload "salza2" :verbose t)|Yes||||
|(ql:quickload "cl-colors" :verbose t)|Yes||||
|(ql:quickload "jonathan" :verbose t)|No||||
|(ql:quickload "proc-parse" :verbose t)|Yes||||
|(ql:quickload "xsubseq" :verbose t)|Yes||||
|(ql:quickload "cl-ansi-text" :verbose t)|Yes||||
|(ql:quickload "clx" :verbose t)|Yes|||https://github.com/sharplispers/clx.git, branch master|
|(ql::quickload :cl-jpeg :verbose t)|Yes|||`(setq clasp-cleavir::*use-ast-interpreter* nil)`|
