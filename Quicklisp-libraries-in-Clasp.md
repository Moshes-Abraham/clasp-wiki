In the following table one can find the state of popular quicklisp distributions in clasp.
Libraries selected according to http://blog.quicklisp.org/2018/03/download-stats-for-february-2018.html

| System | Compiles | Testsuite | Tweaks |
| ------ | ------ | ------ | ------ |
|(ql:quickload "alexandria" :verbose t)|Yes||| 
|(ql:quickload "closer-mop" :verbose t)|Yes|||
|(ql:quickload "babel" :verbose t)|Yes|||
|(ql:quickload "cl-ppcre" :verbose t)|Yes|||
|(ql:quickload "split-sequence" :verbose t)|Yes|||
|(ql:quickload "trivial-features" :verbose t)|Yes|||
|(ql:quickload "iterate" :verbose t)|Yes|||
|(ql:quickload "trivial-gray-streams" :verbose t)|Yes|||
|(ql:quickload "bordeaux-threads" :verbose t)|Yes||Need (https://github.com/sionescu/bordeaux-threads.git , master)|
|(ql:quickload "anaphora" :verbose t)|Yes|||
|(ql:quickload "let-plus" :verbose t)|Yes|||
|(ql:quickload "cffi" :verbose t)|Yes|||
|(ql:quickload "trivial-garbage" :verbose t)|Yes|||
|(ql:quickload "flexi-streams" :verbose t)|Yes|||
|(ql:quickload "nibbles" :verbose t)|Yes||`(setq cmp::*compile-file-parallel* nil)`|
|(ql:quickload "puri" :verbose t)|Yes|||
|(ql:quickload "usocket" :verbose t)|Yes|||
|(ql:quickload "trivial-backtrace" :verbose t)|Yes|||
|(ql:quickload "more-conditions" :verbose t)|Yes|||
|(ql:quickload "chunga" :verbose t)|Yes|||
|(ql:quickload "cl-fad" :verbose t)|Yes|||
|(ql:quickload "cl+ssl" :verbose t)|Yes|||
|(ql:quickload "cl-base64" :verbose t)|Yes|||
|(ql:quickload "esrap" :verbose t)|Yes|||
|(ql:quickload "chipz" :verbose t)|Yes|||
|(ql:quickload "named-readtables" :verbose t)|Yes|||
|(ql:quickload "drakma" :verbose t)|Yes|||
|(ql:quickload "local-time" :verbose t)|Yes|||
|(ql:quickload "ironclad" :verbose t)|Compiling forever||export GC_INITIAL_HEAP_SIZE=40G|
|(ql:quickload "parse-number" :verbose t)|Yes|||
|(ql:quickload "fiveam" :verbose t)|Yes|||
|(ql:quickload "closure-common" :verbose t)|Yes|||
|(ql:quickload "cxml" :verbose t)|Yes|||
|(ql:quickload "log4cl" :verbose t)|No|||
|(ql:quickload "optima" :verbose t)|Yes|||
|(ql:quickload "parser.common-rules" :verbose t)|Yes|||
|(ql:quickload "cl-unicode" :verbose t)|Yes|||
|(ql:quickload "cl-interpol" :verbose t)|Yes|||
|(ql:quickload :lparallel-test) |Yes|(lparallel-test:execute) -> Success: 171 tests, 119190 checks.||
|(ql:quickload "lift" :verbose t)|No|||
|(ql:quickload "cl-dot" :verbose t)|Yes|||
|(ql:quickload "cl-syntax" :verbose t)|Yes|||
|(ql:quickload "cl-annot" :verbose t)|Yes|||
|(ql:quickload "cxml-stp" :verbose t)|No|||
|(ql:quickload "cl-store" :verbose t)|No|||
|(ql:quickload "fare-utils" :verbose t)|Yes|||
|(ql:quickload "fare-quasiquote" :verbose t)|Yes|||
|(ql:quickload "xml.location" :verbose t)|No|||
|(ql:quickload "cl-utilities" :verbose t)|Yes|||
|(ql:quickload "utilities.print-tree" :verbose t)|No|||
|(ql:quickload "trivial-utf-8" :verbose t)|Yes|||
|(ql:quickload "static-vectors" :verbose t)|No|||
|(ql:quickload "fare-mop" :verbose t)|Yes|||
|(ql:quickload "inferior-shell" :verbose t)|No||#\cr|  
|(ql:quickload "quri" :verbose t)|Yes|||
|(ql:quickload "metabang-bind" :verbose t)|Yes|||
|(ql:quickload "trivial-indent" :verbose t)|Yes|||
|(ql:quickload "md5" :verbose t)|Yes|||
|(ql:quickload "documentation-utils" :verbose t)|Yes|||
|(ql:quickload "fast-io" :verbose t)|Yes|||
|(ql:quickload "uuid" :verbose t)|No||ironclad|
|(ql:quickload "array-utils" :verbose t)|Yes|||
|(ql:quickload "plump" :verbose t)|Yes|||
|(ql:quickload "djula" :verbose t)|No|||
|(ql:quickload "symbol-munger" :verbose t)|Yes|||
|(ql:quickload "cl-slice" :verbose t)|Yes|||
|(ql:quickload "collectors" :verbose t)|Yes|||
|(ql:quickload "gettext" :verbose t)|Yes|||
|(ql:quickload "arnesi" :verbose t)|Yes|||
|(ql:quickload "hunchentoot" :verbose t)|Yes|||
|(ql:quickload "access" :verbose t)|Yes|||
|(ql:quickload "cl-locale" :verbose t)|No|||
|(ql:quickload "simple-date-time" :verbose t)|Yes|||
|(ql:quickload "ieee-floats" :verbose t)|Yes|||
|(ql:quickload "prove" :verbose t)|Yes|||
|(ql:quickload "yason" :verbose t)|No|||
|(ql:quickload "asdf-system-connections" :verbose t)|Yes|||
|(ql:quickload "metatilities-base" :verbose t)|No||| 
|(ql:quickload "cl-containers" :verbose t)|No|||
|(ql:quickload "rfc2388" :verbose t)|Yes|||