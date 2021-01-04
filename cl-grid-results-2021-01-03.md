<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en-us">
<body>
	<h1>Load Failures - <a href="http://github.com/cl-test-grid/cl-test-grid">CL Test Grid</a> Report</h1>
    <b>lisp:</b> clasp-cclasp-boehm-0.4.2-3601-g41e03c913-cst-macosx-x64, <b>lib-world:</b> quicklisp 2020-12-20
    <table>
        <thead>
            <tr><th title="ASDF system name.">system-name</th>
                <th title="The ASDF systems preventing the given system to load.">root-blocker-systems</th>
                <th title="The systems, which have the given system as the only root blocker.">systems-blocked-exclusively</th>
                <th title="Projects containing the systems-blocked-exclusively.">projects of the systems-blocked-exclusively</th>
                <th title="Projects depending on the given ASDF system.">dependent-projects</th>
                <th title="ASDF system depending on the given ASDF system.">dependent-systems</th>
            </tr>
        </thead>
        <tbody>
            <tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ovab95zi2">3bgl-shader-example</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cn0548zk2o">3bgl-shader</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xh9ba48yvc">3bz</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ro97xpkd70">3d-matrices-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ltmfnf6ngd">3d-matrices</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=r4olhr2d5q">3d-vectors-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15di53te4y">3d-vectors</a> </td><td>0</td><td>4</td><td>3</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tud9lybrt">a-cl-logger-logstash</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9rfa7uh5w6">a-cl-logger</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tjk5in9yd">aether-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  ERROR during macroexpansion:
    Declaration information is unavailable for this implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gx54ojy7ro">aether</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  ERROR during macroexpansion:
    Declaration information is unavailable for this implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18pwgulsjz">agnostic-lizard-debugger-prototype</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  (FDEFINITION) is an illegal SETF form.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vuqgcxe9j">agnostic-lizard</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  (FDEFINITION) is an illegal SETF form.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xy2uxlxl18">skeleton</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qx64vd5wqr">ahungry-fleece</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qrxqpy1n4">net.mfiano.lisp.algae</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dxoq4z3x3">also-alsa</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBASOUND).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6bx2oc1yga">science-data</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=r1lrq8uwjq">physical-dimension</a> </td><td>1</td><td>0</td><td>0</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13w33z6l1l">foreign-array</a> </td><td>1</td><td>0</td><td>0</td><td>5</td><td>9</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7jkgwxbol5">antik-base</a> </td><td>0</td><td>8</td><td>4</td><td>5</td><td>10</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bon1i4xrgh">antik</a> </td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=l2gpgivxi9">april</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x13ef0b3a1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=127648ka88">arc-compat</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The function COMMON-LISP-USER::QUIT is undefined.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lffcouppd">arrival</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qftvgmh2z">asdf-linguist</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tmlszasd0d">zaserve</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system zaserve from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/aserve-20181210-git/zaserve.asd: Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d33n3ypkn">assert-p</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system assert-p from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/assert-p-20200610-git/assert-p.asd: Could not find package with (nick)name: SIMPLET-ASDF</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=q2dwg3j637">asteroids</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ht5eb6xo4a">atdoc</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in DOLIST:
  (DOLIST (SUB)
    (IF (GOOD-SYMBOL-P (CLASS-NAME SUB) OTHER-PACKAGES)
        (WITH-ELEMENT subclass
                      (RANDOM-NAME (CLASS-NAME SUB) OTHER-PACKAGES class))
        (RECURSE SUB)))</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=32rkbxuq2t">basic-binary-ipc-tests</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tjpm48jbu">beirc</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1311w5svo1">bike-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The variable BIKE-INTERNALS::SIZE is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bfm2ae6v9">bike-examples</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The variable BIKE-INTERNALS::SIZE is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bvnk25tbw">bike</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The variable BIKE-INTERNALS::SIZE is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ol3cgz0kz">binpack-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package :ALEXANDRIA-2</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1je5tcwa7r">bknr.utils</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : missing port for this compiler, please provide for locking primitives for this compiler in /Users/karstenpoeck/lisp/fork-...</span></td><td>0</td><td>4</td><td>1</td><td>2</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5yh2164cs9">bknr.indices</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : missing port for this compiler, please provide for locking primitives for this compiler in /Users/karstenpoeck/lisp/fork-...</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=188kynvdll">bknr.impex</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : missing port for this compiler, please provide for locking primitives for this compiler in /Users/karstenpoeck/lisp/fork-...</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=emhpwpqorc">bknr.datastore</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : missing port for this compiler, please provide for locking primitives for this compiler in /Users/karstenpoeck/lisp/fork-...</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mttmoju5q5">bknr.data.impex</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : missing port for this compiler, please provide for locking primitives for this compiler in /Users/karstenpoeck/lisp/fork-...</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xjf6l80aqz">leech</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ritkeudp56">bknr.web</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;uffi&quot; not found</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8lxrx0l7uw">bknr.modules</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;uffi&quot; not found</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3xw9iep7d2">blackbird-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9a6ek82o6r">bnf.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=n7zlpueulp">bodge-chipmunk</a> <span class="note">CFFI::SIMPLE-FOREIGN-TYPE-ERROR : Detected cycle in type #&lt;ENHANCED-TYPEDEF %CHIPMUNK::SPACE-DEBUG-DRAW-FLAGS&gt;.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nn8h2y8x9">bodge-concurrency</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=apzhizk9lv">bodge-host</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i2tz5a7hf">bodge-math</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=je7wy68sdz">bodge-memory</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wosixh3798">bodge-ode</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not find package with (nick)name: ODE</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ln1erx2zo">bodge-utilities</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dkj3tiex27">bp</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sg80iyd7jg">bt-semaphore-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x6m30boo1f">buildapp</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Too few arguments supplied to a macro or a destructuring-bind form:
  (RUN-PROGRAM (FLATTEN (LIST &quot;--load&quot; (NATIVE-NAMESTRING (PROBE-FILE FILE)))))</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vagts5epnk">buildnode-xul</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kvj7ffl36">buildnode-xhtml</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1s6eqkzr30">buildnode-kml</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tu5q0iu9ec">buildnode-html5</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ykdoflrbl1">buildnode-excel</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dditeydyuk">buildnode</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>0</td><td>11</td><td>3</td><td>4</td><td>12</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1iaumq1y9k">cambl-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ttxij7ocvg">cambl</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dp8oxji76k">can-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14p2zaypty">caramel</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10vb6xow93">cardioex</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t5uxg96g6">carrier</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11htmpskv8">caveman2-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kze0y6ud6">caveman2-db</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1m4lvulnxq">caveman2</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>4</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1iuc8xpgsq">caveman-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qfvwddpm70">caveman-middleware-dbimanager</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1f0chlk67u">caveman</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2gx72rk2ib">caveman2-widgets-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17uygr5rol">caveman2-widgets</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15kxhm0p2w">caveman2-widgets-bootstrap-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9zl0phyx4m">caveman2-widgets-bootstrap</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ei7yrenuds">cepl</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>4</td><td>4</td><td>6</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hbj4a0ax3s">cepl.camera</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=23y2tnbyfg">cepl.devil</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jpwynxf94s">cepl.drm-gbm</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>4</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1v7fiiz7d2">cepl.glop</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7r2yva5k8b">cepl.sdl2</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wxlmd7vu2">cepl.sdl2-image</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mvdah5k2v">cepl.sdl2-ttf</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gnllxtw44n">cepl.skitter.sdl2</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dv31vg139m">cepl.skitter.glop</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9c74ggx4jx">cepl.spaces</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1et8gvte01">ceramic-test-app</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bd4ds0uuwt">ceramic-hello-world</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>5</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1m5dickwl2">ceramic</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t0k43nqc2">cerberus</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gs4vssxn5n">cheat-js</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6crzmkkm71">check-bnf.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19srxj5nh9">check-bnf</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15r3g45slq">chronicity-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1r3oondj6x">chtml-matcher</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qbjgimcyls">city-hash-test</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16zd7lgzep">city-hash</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5voegc29if">cl-acronyms</a> <span class="note">COMMON-LISP:TYPE-ERROR : NIL is not of type NUMBER.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g0hfmfi3l">cl-all</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-POSIX&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xvzb11d4m">cl-amqp.test</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1om158ch1b">cl-amqp</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>2</td><td>0</td><td>0</td><td>2</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5mg2nsnp97">cl-ana.typespec</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fmkq42j89w">cl-ana.typed-table</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1icl3ftxl1">cl-ana.tensor</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bqsmfvqu5a">cl-ana.table-viewing</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pj6tpjfk0">cl-ana.table-utils</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bbf00o7pr">cl-ana.statistics</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18p3lkcwyd">cl-ana.statistical-learning</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nz6uz12oq">cl-ana.serialization</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13lwvzgcr7">cl-ana.quantity</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cc0rixqwks">cl-ana.plotting</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1u6zrmnbo9">cl-ana.ntuple-table</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yfj9or56eg">cl-ana.math-functions</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vnntkkgr9q">cl-ana.makeres-utils</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=inp7vliqd4">cl-ana.makeres-table</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1y1dtngjgz">cl-ana.makeres-progress</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=159w79ia66">cl-ana.makeres-macro</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d3cew5yw7r">cl-ana.makeres-graphviz</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1j55djaucz">cl-ana.makeres-branch</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ibsig3blji">cl-ana.makeres-block</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ngotc52nmj">cl-ana.makeres</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nhy1n5cnsq">cl-ana.lorentz</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12ch21plq4">cl-ana.linear-algebra</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13o9dcnhu8">cl-ana.histogram</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=135hwg8qcg">cl-ana.hdf-utils</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1enygywrv3">cl-ana.hdf-typespec</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dr88mvysl">cl-ana.hdf-table</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=oit9ucaxwb">cl-ana.gnuplot-interface</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17fba0jhvv">cl-ana.fitting</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11k9g0k9ww">cl-ana.file-utils</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ppyx9u2yu">cl-ana.error-propogation</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=613xuzpsih">cl-ana.csv-table</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sxfpcg0nnc">cl-ana.clos-utils</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fud1c2tvg0">cl-ana.calculus</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bmqm5n2ob">cl-ana.binary-tree</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fmgty5rchj">cl-ana</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1q56all4f7">cl-annot-prove-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zy93nyp7d5">cl-annot-prove</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>1</td><td>1</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5uqyd2orli">cl-ascii-art</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cgps11bbds">cl-async-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=u6e4m2s1f6">cl-async-ssl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>4</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16bek1gq25">cl-async-repl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1u3cqvj19l">cl-async</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>9</td><td>14</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=quhy5dfm6l">cl-aubio</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libaubio.so.5&quot; &quot;libaubio.so&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vxh8dh27b">cl-base16</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wjksdvpjy">cl-batis</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19nobtb844">batis-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e01lkts6h">batis</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ewkillt6t">bert</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5c2pqnojkr">bibtex</a> <span class="note">QUICKLISP-CLIENT:SYSTEM-NOT-FOUND : System &quot;port&quot; not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t89eigbnh">cl-bloggy</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6kqmo4lu9j">cl-bson-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nlictn4am">cl-bson</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=109yy8rxcf">cl-bunny.test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vs2gf6o3pa">cl-bunny.examples</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7l96m03s4u">cl-bunny</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>3</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1uyr8n1y6b">cl-cairo2-xlib</a> <span class="note">EXT:UNDEFINED-CLASS : Could not find the class FOREIGN-WRAPPER.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qljfov5z3">cl-cairo2-gtk2</a> <span class="note">EXT:UNDEFINED-CLASS : Could not find the class FOREIGN-WRAPPER.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xn0c7h8sts">capstone</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1r0jljohyb">cl-cffi-gtk-pango</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>10</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d45qtvr0wp">cl-cffi-gtk-opengl-demo</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ex9z6vux27">cl-cffi-gtk-gobject</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>14</td><td>2</td><td>2</td><td>14</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ekg1lqg1zf">cl-cffi-gtk-gio</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>10</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1inr4eeu0g">cl-cffi-gtk-gdk-pixbuf</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>10</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kg4wz7ze9u">cl-cffi-gtk-gdk</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>9</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16u2mv0y6g">cl-cffi-gtk-example-gtk</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13vjwoss0i">cl-cffi-gtk-demo-gobject</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g5drajxsg">cl-cffi-gtk-demo-glib</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hpnk58f7h2">cl-cffi-gtk-demo-cairo</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zor4u467hh">cl-cffi-gtk</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=i2fozx16qu">cl-cheshire-cat</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1etgrxuvcr">cl-clblas-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBCLBLAS).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=o4g5gftf2f">cl-clblas</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBCLBLAS).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10kiehoxd8">net.didierverna.clon.termio</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sv2vaxx46i">net.didierverna.clon.core</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=l0hdxzd69l">net.didierverna.clon</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wn2rk9srgd">cl-clsparse</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libclSPARSE.so&quot; &quot;libclSPARSE.so.1&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ngiudyf6tk">cl-collider</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x11d890ee1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hrqqgmr4qu">cl-conllu</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tmlkellek">cl-coveralls-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tj8sj4u6z">cl-coveralls</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>3</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9efldqvo8c">cl-covid19</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1poxoau7l1">cl-csv-clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1uwogyx3mu">cl-cuda-interop-examples</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=51zhj9auyz">cl-cuda-interop</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lgn8s8iy9e">cl-cuda-examples</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=up350sraw1">cl-cuda</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>3</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1875jx84iu">cl-darksky-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jdi147qdac">cl-darksky</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cf0tevxk2">cl-data-structures-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fqkw20bvfu">cl-data-structures</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qazji9y7x">dbd-mysql</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libmysqlclient.20.dylib&quot; &quot;libmysqlclient.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e0jhfqt5d">dbi-cp-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1opfbwq7qw">dbi-cp</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1eqw0rtjb7">cl-dbi-connection-pool</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lui79g041g">dct-test</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2xrn0j043a">dct</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ejs6xpnl3f">cl-ilut</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libIL.dylib&quot; &quot;libIL.1.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qcz10pl0nq">cl-ilu</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libIL.dylib&quot; &quot;libIL.1.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=e9prmdubm4">cl-devil</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libIL.dylib&quot; &quot;libIL.1.dylib&quot;)</span></td><td>0</td><td>2</td><td>1</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rd4rljvtgh">cl-disque-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ti9oalzhar">cl-disque</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12hr0s5me9">cl-dotenv-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x3hejf8t0i">cl-dotenv</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8n9q2m7nor">cl-drm</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBDRM).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a3w7dtynw">edit-distance-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1w9t3jdoxc">cl-egl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libEGL.so.1&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pnbzykgpdg">enchant-autoload</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (DEFAULT-9922).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=e1dfqo4xv6">cl-environments</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +WALK-MACROS+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=c2oevx23k8">erlang-term</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1is52ibc0a">cl-events.test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b9ilur43e">cl-events</a> </td><td>1</td><td>0</td><td>0</td><td>2</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=93ga8q21tk">cl-fam</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s0y3egbqsf">cl-fastcgi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (PATH &quot;libfcgi.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1shd1vs89j">cl-fbclient</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libfbclient.so.2&quot; &quot;libfbclient.so&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fa1ek1wc9">cl-feedparser-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=53t8qpuqgd">cl-feedparser</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nvfjr8ahha">cl-fix</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ho7c3wtvw">cl-fixtures-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=au7cqvye6i">cl-flowd</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT-CLASS| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fi8vhiowwo">cl-fluent-logger</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6z6f57o4tp">cl-forms.who.bootstrap</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19h0xeh4wl">cl-forms.who</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vtatze351">cl-forms.test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ljvp59wolz">cl-forms.peppol</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11hrllilit">cl-forms.djula</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=axannsn10w">cl-forms.demo</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dcb3fbwh24">cl-forms</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=q20aybrmli">cl-freeimage</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBFREEIMAGE).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=94k4gsoje8">cl-freetype2-tests</a> <span class="note">EXT:UNDEFINED-CLASS : Could not find the class FOREIGN-WRAPPER.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=138l4ccv5h">cl-freetype2</a> <span class="note">EXT:UNDEFINED-CLASS : Could not find the class FOREIGN-WRAPPER.</span></td><td>0</td><td>5</td><td>3</td><td>3</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cdwwd6jdbk">cl-fuse</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBFUSE).
  NIL</span></td><td>0</td><td>2</td><td>2</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=y03ed2equr">cl-fuse-meta-fs</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBFUSE).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1f8mux58cw">cl-gbm</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;/usr/lib64/libgbm.so.1&quot; &quot;/usr/lib64/libgbm.so.0&quot; &quot;/usr/lib64/libgbm.so&quot;
    &quot;/usr/lib/x86_64-linux-gnu/libgbm.so&quot;
    &quot;/usr/lib/x86_64-linux-gnu/libgbm.so.1&quot;
    &quot;/usr/lib/x86_64-linux-gnu/libgbm.so.1.0.0&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2775vvafwc">cl-gd-test</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;uffi&quot; not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rmyde2msdn">cl-gd</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;uffi&quot; not found</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jyko6fc0r">cl-gene-searcher</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dzxm2is453">cl-generator-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4vmorme5ll">cl-geocode</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1h9eb76cn0">cl-geoip</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBGEOIP).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5u6tzcnqui">cl-geos</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libgeos_c.so.1&quot; &quot;libgeos_c.so&quot;)</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=reob1c9rvg">cl-gimei</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t4fsrrk0t">cl-gists-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=twkcgxttvd">cl-gists</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=f6pte4qeob">cl-git</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBGIT2).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ycgt4x10fk">cl-glfw-ftgl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libftgl&quot; &quot;libftgl.so.2&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o1g5lipu1">cl-graph+hu.dwim.graphviz</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libgvc.so&quot; &quot;libgvc.so.4&quot; &quot;libgvc32.so.4&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13uuzhxx8n">cl-gserver</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vj0ekwpho">cl-gtk2-pango</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3dchf835kb">cl-gtk2-gtk</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1up3hqujl2">cl-gtk2-glib</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>7</td><td>2</td><td>3</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=b6nfdqcv9y">cl-gtk2-gdk</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ajuu857k72">cl-gtk2-cairo</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nrs6dq7n2">cl-html-readme-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kv0dy66xe2">cl-htmlprag</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17n4vlemgp">cl-i18n</a> <span class="note">ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-NOT-BE-FIRST : A symbol token must not start with two package markers as in ::name.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kay9xhqmrj">cl-influxdb</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT-CLASS| is unbound.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ij11owi8s5">cl-inotify-tests</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-inotify from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-inotify-20200427-git/cl-inotify.asd: Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zi5themblc">cl-inotify</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-inotify from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-inotify-20200427-git/cl-inotify.asd: Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1zr2fabwd3">cl-irc-test</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not find package with (nick)name: CL-IRC-TEST</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=v8871z7oir">cl-k8055</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBK8055).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bdjgmfs01">cl-kanren-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wxcxp3dii">cl-kanren</a> </td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1f4jrqd8su">kaputt</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jnwo0tmyd7">cl-kyoto-cabinet</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBKC).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hyj6x4b135">cl-l10n</a> <span class="note">EXT:STREAM-DECODING-ERROR : decoding error on stream
#&lt;IOFILE-STREAM #P&quot;/Users/karstenpoeck/lisp/fo... file-pos 1&gt;
(:EXTERNAL-FORMAT NIL):
  the octet sequence (190) cannot be decoded.</span></td><td>0</td><td>3</td><td>3</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ni7w3sllmp">langutils</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=v23nsfcwba">cl-lastfm-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qgesad1a1">cl-ledger</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=frqm05wohx">cl-lexer</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=181luawj9k">cl-liballegro</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;liballegro.5.2.6.dylib&quot; &quot;liballegro.5.2.dylib&quot; &quot;liballegro.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8m82hrjpin">cl-liballegro-nuklear</a> <span class="note">UIOP/RUN-PROGRAM:SUBPROCESS-ERROR : Subprocess with command &quot;make -f /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-liballegro-nuklear-20201220-git/src/Makefile&quot;
 exited with error code 512</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ohtjl7dmu">cl-libevent2-ssl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libevent_core.dylib&quot; &quot;/usr/local/lib/libevent_core.dylib&quot;
    &quot;/opt/local/lib/libevent_core.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=uepmiqqfws">cl-libevent2</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libevent_core.dylib&quot; &quot;/usr/local/lib/libevent_core.dylib&quot;
    &quot;/opt/local/lib/libevent_core.dylib&quot;)</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vxijt1icrx">cl-libhoedown</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Unable to load any of the alternatives:
     (&quot;libhoedown.dylib.3&quot; &quot;libhoedown.dylib&quot; &quot;libhoedown.so.3&quot; &quot;libhoedown.so&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yr7v7b77sv">cl-libiio</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBIIO).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3unplbiu29">cl-libpuzzle-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libpuzzle.so.1&quot; &quot;libpuzzle.so&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fntpl3eyf">cl-libpuzzle</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libpuzzle.so.1&quot; &quot;libpuzzle.so&quot;)</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t1qzqw7v1">libssh2.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12fdcfb81&gt;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vhurzkvzpc">libssh2</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBSSH2).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10lwyiyc9o">cl-libsvm</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBSVM).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10imi8xnsa">cl-liblinear</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBLINEAR).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=105iq5p22t">libusb-ffi</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8tdh365n2d">cl-libusb</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18ouczlcut">cl-libuv</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>0</td><td>12</td><td>7</td><td>9</td><td>17</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x1n8b24g9v">cl-libyaml-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ux0fnvfnuj">cl-libyaml</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>0</td><td>6</td><td>4</td><td>4</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8r39fm3nj8">cl-locale-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6p0v3c0tod">cl-locale-syntax</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=101h6jyhlg">cl-locale</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lxi38llb71">cl-logic</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-INTROSPECT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gcc281hy7c">lzlib-tests</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;liblz.so&quot; &quot;liblz.so.1&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jrwinj48x7">lzlib</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;liblz.so&quot; &quot;liblz.so.1&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vgprm9bldi">cl-m4-test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vavstjl0e">cl-m4</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jgpcxujpj">marshal-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Error: Name conflict for USE-PACKAGE of [XLUNIT] by package[COMMON-LISP-USER]
   - conflicting symbols:  &quot;TEST&quot;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d4xufpy9qe">cl-match-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  ERROR during macroexpansion:
    HAS-LENGTH is not of type LIST.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ahyyytu8g">cl-match</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  ERROR during macroexpansion:
    HAS-LENGTH is not of type LIST.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ba0gyguc6r">cl-mechanize</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Implementation not supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nkav4g6wu9">cl-messagepack-rpc-tests</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hj502xiuh">cl-messagepack-rpc</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jshnt9kjzd">cl-migrations</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1n4kr7diss">cl-migratum.test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1m68kfxj37">cl-migratum.provider.local-path</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tzfvo5evz5">cl-migratum.driver.sql</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8mg3xia79f">cl-migratum</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vdp052scd0">mlep-add</a> <span class="note">ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-NOT-BE-FIRST : A symbol token must not start with two package markers as in ::name.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13c8d65tax">mlep</a> <span class="note">ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-NOT-BE-FIRST : A symbol token must not start with two package markers as in ::name.</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cz85gvqo5b">modlisp</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;modlisp&quot; not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1btc63ybxd">cl-mongo</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;IRONCLAD&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pgpx2s7i9">cl-mongo-id</a> <span class="note">COMMON-LISP:UNDEFINED-FUNCTION : The function CL+SSL::PTR is undefined.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=psrhxxvyxn">cl-mop</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The name &quot;CLASS-SLOTS&quot; does not designate any package</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=106411j3io">cl-mpi-test-suite</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;mpicc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 32512</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ni90ra6de">cl-mpi-extensions</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;mpicc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 32512</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9lroohlabj">cl-mpi-examples</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;mpicc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 32512</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tund1sjpp">cl-mpi</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;mpicc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 32512</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18o9pv4d2x">mssql</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (SYBDB).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pauqxis0ez">cl-mtgnet-async</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tkbb7xmp3">cl-mw.examples.with-task-policy</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hx7q4ghms">cl-mw.examples.ping</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1c3c45pt3q">cl-mw.examples.monte-carlo-pi</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4c9cbllt2c">cl-mw.examples.higher-order</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=twwozczlgh">cl-mw.examples.hello-world</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=npfrbsnqa7">cl-mw.examples.argument-processing</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zavz423u61">cl-mw</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1juok7usmn">cl-mysql-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libmysqlclient.20.dylib&quot; &quot;libmysqlclient.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i2kqjm8on">cl-mysql</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libmysqlclient.20.dylib&quot; &quot;libmysqlclient.dylib&quot;)</span></td><td>0</td><td>2</td><td>2</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hh38c9p4c">cl-ncurses</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;uffi&quot; not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1riywscbxx">cl-neovim</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b3att5r8e">cl-notebook</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The name &quot;CLASS-SLOTS&quot; does not designate any package</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=150yoft6jj">nxt-proxy</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : no frame pair found of name NXT-OPEN-READ</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6lp5ys5sg8">nxt</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : no frame pair found of name NXT-OPEN-READ</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d77kos4x7y">cl-oclapi-test</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type CL-BITFIELD</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=js3mha9e8b">cl-oclapi</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>1</td><td>1</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11g93bkc99">cl-ode</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libode.so&quot; &quot;libode.so.1&quot; &quot;libode.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lnkm4ti9m">cl-ohm</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5dgd85hdwf">cl-online-learning-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hcjw39bw1">cl-online-learning</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1be7sqq6n5">cl-openal-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:DEFAULT &quot;libalut&quot;) (:FRAMEWORK &quot;alut&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=62n2ejrpvd">cl-alut</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:DEFAULT &quot;libalut&quot;) (:FRAMEWORK &quot;alut&quot;))</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1eoh4u38l4">or-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (GLPK).
  NIL</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=u5ydlegwbm">or-gsl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (GSLCBLAS).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=188ymxisko">or-glpk</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (GLPK).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1osegjsl5g">or-fann</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (FANN).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tyyq9tonvg">cl-pattern-benchmark</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=in1f0nfxm8">cl-pattern</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>4</td><td>3</td><td>7</td><td>16</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8y5gcihapj">cl-plplot</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBPLPLOT).
  NIL</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zhugechdpo">cl-plumbing-test</a> <span class="note">CORE:SIMPLE-READER-ERROR : Undefined reader macro for char &#039;#&#039; subchar &#039;&gt;&#039; in file fifo-pipe.lisp line: (23) column (6).</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4jbn5t9ydj">cl-plumbing</a> <span class="note">CORE:SIMPLE-READER-ERROR : Undefined reader macro for char &#039;#&#039; subchar &#039;&gt;&#039; in file fifo-pipe.lisp line: (23) column (6).</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13btypcfxu">cl-ply-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=b8c8vlnypv">cl-ply</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mr1r4i8ff">cl-portaudio</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBPORTAUDIO).
  NIL</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1h82atxssw">cl-project-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s37hdp0qxv">cl-prolog2.yap.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=uw95lplpug">cl-prolog2.yap</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i7xg2qhka">cl-prolog2.xsb.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=190hk72knf">cl-prolog2.xsb</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xthesvenn">cl-prolog2.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vptrvfwqj0">cl-prolog2.swi.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1c1misgp1s">cl-prolog2.swi</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=57lmubqunh">cl-prolog2.gprolog.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=doyi7pne0z">cl-prolog2.gprolog</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14rdu4y2kh">cl-prolog2.bprolog.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hm8rviefp">cl-prolog2.bprolog</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kpg7nsj0su">cl-prolog2</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pgqw3wz375">cl-protobufs-tests</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tyruwob1di">cl-pslib</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBPS).
  NIL</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j005e5ie4g">cl-pslib-barcode</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBPS).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=owya7n7mlt">clpython</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  A CHECKING-READER-CONDITIONALS expression returned zero forms, in: /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-python-20200427-git/util/utils.lisp</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8wct9arciz">cl-qrencode-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=b116lrihdc">cl-rabbit-tests</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-I/usr/local/include&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fgs8crspji">cl-rabbit</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-I/usr/local/include&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5k4h7u9tn1">cl-random</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBRMATH).
  NIL</span></td><td>3</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1djct7t8ol">cl-random-forest-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=35z0ftb920">cl-random-forest</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ct55yu969">cl-rdkafka</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-I&quot; &quot;/usr/local/include&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g54dbp8a6">cl-redis</a> </td><td>1</td><td>0</td><td>0</td><td>4</td><td>7</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=unqwmirfl0">cl-renderdoc</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBRENDERDOC.SO-14552).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mhmvalmkj">cl-rethinkdb-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ur3kasi9f">cl-rethinkdb</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1skgdbsohk">cl-rmath</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBRMATH).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=39empc01cj">cl-rrd</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;librrd.so.2&quot; &quot;librrd.so&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mv8cewgu1w">cl-rrt.test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bffjgo8un">cl-rrt.rtree</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ezm6p9efk">cl-rrt.benchmark</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=y52mo5g1p7">cl-rrt</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>3</td><td>1</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jrs1f1m951">rss</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=43ye8hwqds">cl-rsvg2-test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xrebpkms4r">cl-rsvg2-pixbuf</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b5nk60as9">cl-rsvg2</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=k0bn4rvsp9">cl-rules-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kyc63wwrut">cl-rules</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1is74lbq0z">cl-sam-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=c67ygap3az">cl-sam</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nmkjth6rw">sane</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libsane.so.1&quot; &quot;libsane.so&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a4hm203lv">cl-sat.glucose.test</a> <span class="note">QUICKLISP-CLIENT:SYSTEM-NOT-FOUND : System &quot;cl-sat.glucose&quot; not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tn3v72rfez">cl-sat.minisat.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : none of the installation options are available! Supported packaging systems:
(APT DNF YUM PACMAN YAOURT BREW MACPORTS FINK CHOCO)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lk7dy8mkq6">cl-sat.minisat</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : none of the installation options are available! Supported packaging systems:
(APT DNF YUM PACMAN YAOURT BREW MACPORTS FINK CHOCO)</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4rfirkiazz">cl-scrobbler</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sz5r70wdcn">sdl2-image</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;SDL2_image&quot;) (:DEFAULT &quot;libSDL2_image&quot;))</span></td><td>0</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b2z72rrdg">sdl2-mixer</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;SDL2_mixer&quot;) (:DEFAULT &quot;libSDL2_mixer&quot;))</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1haysmt0dl">sdl2-ttf-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;SDL2_ttf&quot;) (:DEFAULT &quot;libSDL2_ttf&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lx46ij1zy">sdl2-ttf</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;SDL2_ttf&quot;) (:DEFAULT &quot;libSDL2_ttf&quot;))</span></td><td>0</td><td>1</td><td>1</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1caibgvwpk">sendgrid</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15vz2fcxz5">shlex</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ic4zze26s">cl-skip-list</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=49jqa7dvzw">cl-skkserv</a> <span class="note">ESRAP:INVALID-EXPRESSION-ERROR : Invalid expression: (CHARACTER-RANGES (#0 #9))</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3pydy2svh1">cl-slp</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libslp.so&quot; &quot;libslp.so.1&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=23299qb64l">cl-soloud</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tytgbqrfp">cl-sophia</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBSOPHIA).
  NIL</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tylpglcf9">cl-ssdb-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ohd5qlewvo">cl-ssdb</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a23ggy8pw">cl-statsd.test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=oid0nfxbz1">cl-statsd</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=77i0o3nnz1">cl-store</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>16</td><td>9</td><td>15</td><td>29</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=199nt8new2">cl-strftime</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ehnjzm9qgw">cl-string-match-test</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;FOO-RANDOM&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19o3w5eq1u">cl-string-match</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;FOO-RANDOM&quot; does not exist.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dmlx45kkh">cl-syntax-clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17ggztasoa">cl-tasukete-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kz0aty1lq">cl-tasukete</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vms9d7oow">tcod</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBTCOD).
  NIL</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g7zgqudzb">parse-rgb</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBTCOD).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12h31mqm3u">cl-telegram-bot</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14y7fxw9ef">cl-tetris3d</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qadcwrx3a">cl-threadpool-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19slqxxwws">cl-tiled</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dz0vl48mk">cl-tokyo-cabinet-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBTC).
  NIL</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6bpajlcqbg">cl-tokyo-cabinet</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBTC).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19y4qjfo4f">torrents-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nlb1t8nadm">torrents</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sbwyogh95c">cl-transmission-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vhh6l7fjuo">cl-transmission</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lkw5uesy2f">cl-twit-repl</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not find package with (nick)name: CL-TWIT-REPL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9iwhbjk886">unix-sockets.tests</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=trlqrymul5">unix-sockets</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3kfs5sdzff">gt</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wqa1fygjmu">cl-vhdl</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Row-major array index 0 is out of bounds (INTEGER 0 (0)).</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6rhzkxk7o9">cl-video-player</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBPORTAUDIO).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xclsxclxs3">cl-voxelize-examples</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hmxqqaq9mu">cl-wayland</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (WAYLAND-SERVER).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7c7g6hta6s">cl-weather-jp-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kj0wxhpo66">cl-weather-jp</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1aew7dig7j">cl-webdav</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +DAV-PROPERTY-ALIST+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xgikpi89v4">cl-webkit2</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rbpnh03lq4">cl-why</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +NEWLINE+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1q9a51l605">cl-xkb</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;/usr/lib64/libxkbcommon.so.0&quot; &quot;/usr/lib64/libxkbcommon.so&quot;
    &quot;/usr/lib/x86_64-linux-gnu/libxkbcommon.so&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4haws7deh3">cl-xul-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ze611wgptu">cl-xul</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vnnll4f6zk">cl-yaclyaml</a> </td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17gnzluapy">cl-yaml-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kzuxo85hi">cl-yaml</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10p669ch9g">cl-yesql</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d8zd7ekgj">zyre</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libzyre.dylib&quot; &quot;libzyre.2.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yl21p0hrb8">clache-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ly3zl0s72z">clache</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>2</td><td>0</td><td>0</td><td>5</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yx383fzfxl">t-clack-v1-compat</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a51mvyzsr">t-clack-middleware-csrf</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mfxlmg4ht">t-clack-middleware-auth-basic</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ctj2f5ck3">t-clack-handler-wookie</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lhsdboky9">t-clack-handler-toot</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i1idvv9d3">t-clack-handler-hunchentoot</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1uwmmguyjf">t-clack-handler-fcgi</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vaw4i2bt8a">clack-v1-compat</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>4</td><td>2</td><td>6</td><td>13</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tmvnz1imm">clack-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ixgop1rtfa">clack-session-store-dbi</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18ea1e4hn4">clack-middleware-rucksack</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d9z3pa8s6">clack-middleware-postmodern</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ijc96o3xxx">clack-middleware-oauth</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jphmzfizdd">clack-middleware-dbi</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ic211lyne">clack-middleware-csrf</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1whu013wgf">clack-middleware-clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nemzi4q6mu">clack-middleware-auth-basic</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vz181ev7n">clack-handler-wookie</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1gq7a1ds31">clack-handler-fcgi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (PATH &quot;libfcgi.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1m4qqec8fx">lack-middleware-clack-errors</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xqbjh8zhum">clack-errors-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16dpwe5fur">clack-errors-demo</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rsraxr6y6">clack-errors</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>9</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s6ppk7qncr">clack-pretend</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1sayz289du">clack-static-asset-middleware-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1470eb50rq">clack-static-asset-djula-helpers</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wqoclrfbu">clad</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +CL-SUBFOLDER-NAME+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=in0rjtqoo3">classimp-samples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (ASSIMP).
  NIL</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j41hjgf2il">classimp</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (ASSIMP).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1gthzx1hu1">clath</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=it738rbcal">clavatar</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e8p1e3edx">clavier.test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=io3wkx9145">clavier</a> </td><td>0</td><td>2</td><td>2</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qwkbx6uwh">clawk</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ee3iuse5e">clazy</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system clazy from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/clazy-20200218-git/clazy.asd: Too few arguments supplied to a macro or a destructuring-bind form:
(:FILE)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=txb4saj2aw">clem-test</a> <span class="note">COMMON-LISP:UNDEFINED-FUNCTION : The function CLASS-DIRECT-SUPERCLASSES is undefined.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=972467v80t">clem-benchmark</a> <span class="note">COMMON-LISP:UNDEFINED-FUNCTION : The function CLASS-DIRECT-SUPERCLASSES is undefined.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xbvlqc3572">clem</a> <span class="note">COMMON-LISP:UNDEFINED-FUNCTION : The function CLASS-DIRECT-SUPERCLASSES is undefined.</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j9ma6vgque">cleric</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14xy8vcl1f">clesh-tests</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rhjct2vna">cletris-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libSDL-1.2.so.0&quot; &quot;libSDL-1.2.so&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=epy9k3avsw">cletris-network</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libSDL-1.2.so.0&quot; &quot;libSDL-1.2.so&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=20wpwebk9h">cletris</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libSDL-1.2.so.0&quot; &quot;libSDL-1.2.so&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=963r0uptou">clfswm</a> <span class="note">ECLECTOR.READER:READ-TIME-EVALUATION-ERROR : Read-time evaluation of expression (CONCATENATE &#039;STRING
                                                &quot;Version: 13??   built &quot;
                                                (DATE-STRING)) signaled SIMPLE-TYPE-ERROR: Not a condition type: TOOLS::NOT-IMPLEMENTED</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=k48uvfk9hl">clim-widgets</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p5cu3nwi3">climc-test</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1f468stv1q">climc</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1y0ef8jci2">climon-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libSDL-1.2.so.0&quot; &quot;libSDL-1.2.so&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=169cf9b5e1">climon</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libSDL-1.2.so.0&quot; &quot;libSDL-1.2.so&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=anthslvz7z">clinch-pango</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak key-or-value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=v1ul7raj2p">clinch-freeimage</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak key-or-value hash-tables.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1n8xc4u3lt">clinch-classimp</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (ASSIMP).
  NIL</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1x4opbv68s">clinch-cairo</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak key-or-value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9ijvzzhbmz">clinch</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak key-or-value hash-tables.</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1sy3wfpeqp">clipper-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j3p5h6a58s">clipper</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=e5myjixr90">clite</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Cannot export the symbol STR
  from #&lt;PACKAGE CORE&gt;,
  because it will cause a name conflict
  in #&lt;PACKAGE COMPILER&gt;.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tym43h4cc">clj</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  (FDEFINITION) is an illegal SETF form.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d465e13e3">fork-future</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=osk0izlqov">clml.utility</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Too few arguments supplied to a macro or a destructuring-bind form:
  (DEFPARAMETER *CSV-DEFAULT-EXTERNAL-FORMAT*)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1n5m29nfwy">clml.time-series</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ef9st9w1w3">clml.text</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o51gcrufk">clml.test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jeailc3cu">clml.svm</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1otkfkexoj">clml.statistics.rand</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The variable W is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kwhaqwc2di">clml.statistics</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The variable W is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1y1fg2wvql">clml.som</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=c6rzcnyiix">clml.pca</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1svvmjn80p">clml.numeric</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yim2fl5le2">clml.nonparametric</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o1orvwzh8">clml.nearest-search</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6u89gjsv50">clml.lapack</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=me2rjjooqk">clml.hjs</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17syrq8lbq">clml.graph</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1k7rvc89d7">clml.docs</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=f50cru5dft">clml.decision-tree</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=186bgldjg4">clml.data.r-datasets</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sjb62jefj7">clml.data</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vgdkblsdl">clml.clustering</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ig2hk71yu">clml.classifiers</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15i1dry4oq">clml.association-rule</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pmm6kajlm">clml</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1s5lvwhoes">clonsigna</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cmlguhxdji">clsql-uffi</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19l8snehrn">clsql-tests</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1m8kz5cn14">clsql-sqlite3</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lky6s7rhs">clsql-sqlite</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fmz6e75na5">clsql-postgresql-socket3</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=op0afq0id9">clsql-postgresql-socket</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=erm0m70kdn">clsql-postgresql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18q80mt0kx">clsql-odbc</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=90kjo6aohu">clsql-mysql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kqu05snw11">clsql-cffi</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  The function FINALIZE-INHERITANCE is undefined.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hbky9w0gn">clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>15</td><td>30</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tivo8gxkh">clsql-fluid</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14gf6ity6r">clsql-helper-slot-coercer</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ghs4nmd86d">clsql-helper</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>4</td><td>7</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xhixu8oqd">clsql-local-time</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hb2idl7ng">clsql-orm</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dqmr0qhap">clweb</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : NIL is not a valid pathname-:HOST component</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17dqznqa6f">clws</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xsdqkb091b">cmd</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18fe2difxq">codex-templates</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6wdu5gvdka">codex</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lb0jay8z1">coleslaw-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rhs88x35xo">coleslaw-cli</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7676csmmtb">coleslaw</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=buc128auop">liter</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12kf4vtm70">garten</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wuenw3f194">colliflower-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p2x3k6d8p">colliflower-fset</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wma36px7e1">colliflower</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s3ddiblsxn">colored-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Could not find the class COLOR.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3mfd2g1vrh">colored</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Could not find the class COLOR.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ptgvsy0cx">com.clearly-useful.generic-collection-interface.test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xdmwj0vf6k">com.clearly-useful.generic-collection-interface</a> </td><td>1</td><td>0</td><td>0</td><td>3</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1q8we8038u">com.clearly-useful.iterate+</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tl0hxvwl7">com.clearly-useful.iterator-protocol</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fzp1a04wro">com.clearly-useful.protocols</a> </td><td>0</td><td>4</td><td>3</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1eo1erl9rh">qt-tutorial</a> <span class="note">ASDF/BACKWARD-INTERFACE:OPERATION-ERROR : OPERATION-ERROR while invoking #&lt;COMPILE-OP &gt; on #&lt;CPP-&gt;SO &quot;qt&quot; &quot;so&quot; &quot;commonqt&quot;&gt;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lm1ckt1sv">qt-test</a> <span class="note">ASDF/BACKWARD-INTERFACE:OPERATION-ERROR : OPERATION-ERROR while invoking #&lt;COMPILE-OP &gt; on #&lt;CPP-&gt;SO &quot;qt&quot; &quot;so&quot; &quot;commonqt&quot;&gt;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cbaqm3pcz">qt-repl</a> <span class="note">ASDF/BACKWARD-INTERFACE:OPERATION-ERROR : OPERATION-ERROR while invoking #&lt;COMPILE-OP &gt; on #&lt;CPP-&gt;SO &quot;qt&quot; &quot;so&quot; &quot;commonqt&quot;&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1eqo9ns50w">qt+libs</a> <span class="note">EXT:ASSERT-ERROR : The assertion (UIOP/UTILITY:LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mb38ybrhw7">qt</a> <span class="note">ASDF/BACKWARD-INTERFACE:OPERATION-ERROR : OPERATION-ERROR while invoking #&lt;COMPILE-OP &gt; on #&lt;CPP-&gt;SO &quot;qt&quot; &quot;so&quot; &quot;commonqt&quot;&gt;</span></td><td>0</td><td>4</td><td>2</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nqvoinidco">configuration.options-syntax-xml</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a0osvqxfn">configuration.options-syntax-ini</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j3wpx1hptx">configuration.options-source-commandline</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1k5x8j5m6y">configuration.options-and-service-provider</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mw71an3og">configuration.options-and-quri</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2th3fmvk33">configuration.options-and-puri</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zwqi2khhsp">configuration.options-and-mop</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=f99s614iy7">configuration.options</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a94c7905d">core-reader.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wddmocgfn">corona-web</a> </td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x731mlk3eq">corona-test</a> </td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=m03tdtlafu">corona</a> </td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=80svksx4g9">crane-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6ins36wnwt">crane</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14qy9tapws">croatoan-test</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=knq3a3ibdz">croatoan-ncurses</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ow3zanh4rv">croatoan</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zawb76qdja">ansi-escape-test</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-POSIX&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19l0kl6km0">ansi-escape</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-POSIX&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qbhpeuf0s">css-lite</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11vs22aaej">css-selectors-stp</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ofeoqutqqw">css-selectors-simple-tree</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=z2vk21s7bu">css-selectors</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gouwgiqd3d">cxml-rng</a> <span class="note">COMMON-LISP:TYPE-ERROR : #&lt;EMPTY  @0x12a22bac1&gt; is not of type %TYPED-PATTERN.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rcm4hra5h">priority-queue-benchmark</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Structure definition for NODE cannot have :NAMED without :TYPE.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b1jn60wk4">darts.lib.message-pack-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Invalid function name: (ERROR &quot;octet streams not supported in this implementation&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=f37fcoc05b">data-lens</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kkpixmifs">data-table-clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=q1c354iijm">datafly-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3klpnzt7ct">datafly</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=aee3821rs5">dataloader.test</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-I/usr/include&quot; &quot;-I/usr/local/include&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a24jb8j38">dataloader</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-I/usr/include&quot; &quot;-I/usr/local/include&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zvwdy3plje">dbus</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=l12w8w3w7b">wilbur</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  No locking defined (WITH-LOCK)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x4vylsqmq7">deeds</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qhj8gj0m5">deoxybyte-gzip-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13vtwksx5j">deoxybyte-gzip</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=n3r5tkqtgv">deoxybyte-io-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o476gzfpj">deoxybyte-io</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>0</td><td>7</td><td>4</td><td>5</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13l3si8qsl">deoxybyte-unix-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17ldvl9nzn">deoxybyte-unix</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xezcbq5c9">deoxybyte-utilities-test</a> <span class="note">ECLECTOR.READER:UNKNOWN-CHARACTER-NAME : Unrecognized character name: &quot;FormFeed&quot;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18blgrsagh">descriptions.validation</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1q68pslxhs">descriptions.serialization</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17f214dbs3">descriptions-test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vak6wfv2f0">descriptions</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=w08lzvriey">destructuring-bind-star</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pqd1v3z64">dexador-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16ezc180yw">diff-match-patch</a> <span class="note">COMMON-LISP:SIMPLE-TYPE-ERROR : 1266651024 is not a proper list</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pzz9puc71b">dirt</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11a4uyep1n">djula-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bbihz4duj">djula-demo</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dlu4x51sa3">djula</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>7</td><td>2</td><td>5</td><td>15</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s7osu5mupq">drakma-async</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=59dahrdl58">duologue</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xmmq64df6">easing-demo</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;SDL2_image&quot;) (:DEFAULT &quot;libSDL2_image&quot;))</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=62w4g0p4ry">easy-routes+djula</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zdl91i4exw">eazy-documentation</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-KERNEL&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jxtatxl429">eazy-process.test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4uxua3m20m">eazy-process</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wbm1ck7jdd">eazy-project.test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9kdfajxqnz">eazy-project.autoload</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1s9kpbq7gu">eazy-project</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=whl0a4k2f3">ec2</a> <span class="note">COMPAT:NOT-IMPLEMENTED : Missing implementation: (GETENV AWS_ACCESS_KEY_ID)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vv76o3fulh">eclector-concrete-syntax-tree</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17d4ux00sx">eclector</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=deullew5ey">elb-log-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gmnt1u3aej">elb-log</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1v34x5m9g1">ernestine-tests</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1sgjalv4my">ernestine</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tndqtg98o">erudite-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7ltlj0kv6n">erudite</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1r8lfw9jrp">esrap-liquid</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Row-major array index 0 is out of bounds (INTEGER 0 (0)).</span></td><td>0</td><td>3</td><td>2</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lvtaz91do">eventfd</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ddp15sfez">evol-test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i6hdkrt90">evol</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1uot5r77zy">exit-hooks</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Too few arguments supplied to a macro or a destructuring-bind form:
  (DEFINE-SYMBOL-MACRO *EXIT-HOOKS*)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2yikok1a90">exscribe</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  ERROR during macroexpansion:
    too many arguments</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1smlbcxltl">ext-blog</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=eylw5jky30">external-program</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>10</td><td>8</td><td>14</td><td>29</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=109duyay59">lapack</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=160fi78un8">hompack</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=evb5z4feup">fare-scripts</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kh1xlw8o9">fast-generic-functions-test-suite</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Not a valid initarg: &#039;LEAF-METHOD-P</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1w8ejsrkt1">fast-http-test</a> <span class="note">CORE:SIMPLE-READER-ERROR : Undefined reader macro for char &#039;#&#039; subchar &#039;?&#039; in file benchmark.lisp line: (16) column (40).</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qzwopfkxd">net.scipolis.graphs</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure
(((CAR PINNED-OBJECTS))
 (EXECUTE-THUNK-WITH-PINNED-OBJECTS THUNK (CDR PINNED-OBJECTS)))
according to ((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: NIL @0x13038a7c1&gt; is not a CONS-CST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9l5c58kesl">femlisp-picture</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;uffi&quot; not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=noenhjt2iv">femlisp-parallel</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure
(((CAR PINNED-OBJECTS))
 (EXECUTE-THUNK-WITH-PINNED-OBJECTS THUNK (CDR PINNED-OBJECTS)))
according to ((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: NIL @0x12a463861&gt; is not a CONS-CST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=l1gefg0lez">femlisp-matlisp</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure
(((CAR PINNED-OBJECTS))
 (EXECUTE-THUNK-WITH-PINNED-OBJECTS THUNK (CDR PINNED-OBJECTS)))
according to ((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: NIL @0x121bba3b1&gt; is not a CONS-CST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9w1wytlanw">femlisp-dictionary</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure
(((CAR PINNED-OBJECTS))
 (EXECUTE-THUNK-WITH-PINNED-OBJECTS THUNK (CDR PINNED-OBJECTS)))
according to ((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: NIL @0x122d8ed61&gt; is not a CONS-CST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b5qotbtjf">femlisp-basic</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure
(((CAR PINNED-OBJECTS))
 (EXECUTE-THUNK-WITH-PINNED-OBJECTS THUNK (CDR PINNED-OBJECTS)))
according to ((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: NIL @0x126a51221&gt; is not a CONS-CST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=th5uon5c2l">femlisp</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure
(((CAR PINNED-OBJECTS))
 (EXECUTE-THUNK-WITH-PINNED-OBJECTS THUNK (CDR PINNED-OBJECTS)))
according to ((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: NIL @0x130ee42b1&gt; is not a CONS-CST.</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dbjy42b4ca">dealii-tutorial</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure
(((CAR PINNED-OBJECTS))
 (EXECUTE-THUNK-WITH-PINNED-OBJECTS THUNK (CDR PINNED-OBJECTS)))
according to ((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: NIL @0x127bd6ee1&gt; is not a CONS-CST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nwot7xicp">ddo</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zquzrgxhq5">cl-cpu-affinity</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-cpu-affinity from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/femlisp-20201016-git/external/cl-cpu-affinity/cl-cpu-affinity.asd: CL-CPU-AFFINITY is Linux only.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8w9tx603yi">flare-viewer</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11vxn44odf">flare</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bqqxf3xox3">floating-point-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wogchlb34m">flow-visualizer</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system flow-visualizer from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/flow-20200610-git/visualizer/flow-visualizer.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17cy5m9y3q">folio2-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1v6s8438qd">folio2-taps-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kxtksf42ug">folio2-taps</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5jnsq614xu">folio2-series-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ge5fka0cg">folio2-series</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hbbo0ekcyj">folio2-sequences-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7gokz86cje">folio2-sequences-syntax</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12q41bprf4">folio2-sequences</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=g71o1sjx2f">folio2</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=73v9874b7a">format-string-builder</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5apsi6mw00">formlets-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  &quot;Results&quot; is not of type LIST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1j4wga3sig">frpcgen</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11bmtnly6p">frpc</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1gqmj8qhb6">function-cache-clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dsducst5qf">functional-trees</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14j71au5ik">fxml</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=n8tia8rvgx">yadd</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1axg7y2sfe">wire-world</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6x4q1l70qj">tree</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=krlk677sca">translators</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rozlbf9kz">tasty</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=az6kwj7vke">ta2</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fcyhaoqr7">setup-cffi</a> <span class="note">COMMON-LISP:TYPE-ERROR : NIL is not of type (OR STRING PATHNAME).</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j4m2zdvuxh">robot</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=u424dhknxv">regression</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7xka0lhpgn">ledger</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=g9z79ixkro">gwl-graphics</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>12</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=o11w1c32su">gwl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>16</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16hqkhpt0d">graphs</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15lnq6rtf0">gendl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i3c3toqtn">dom</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gln1067n7z">bus</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e6gufeyzw">generic-cl.util</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Cannot export the symbol CLOSER-MOP:STANDARD-GENERIC-FUNCTION from #&lt;PACKAGE CLOSER-ENVIRONMENTS&gt;,
  because there is already a symbol with the same name
  in the package.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=116x8uxx7n">generic-cl</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +OPTIMIZE-QUALITIES+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=c206622bvc">open-geneva</a> <span class="note">eclector.reader:package-does-not-exist : Package named &quot;[&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dzq1hhv46b">geneva-html</a> <span class="note">eclector.reader:package-does-not-exist : Package named &quot;[&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bwccsy4ji">gettext-example</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qj8jo3yp2">glaw-sdl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ktczlzmpmd">glaw-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (BRIDGE).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a9u4nb4tk">glisph-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wxqdasn1no">glisph</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hb8a14aoi">glop-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (BRIDGE).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nykaq1hosb">glop</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (BRIDGE).
  NIL</span></td><td>0</td><td>3</td><td>3</td><td>3</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1u4csmwscm">gsll</a> </td><td>1</td><td>0</td><td>0</td><td>4</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=33chv5oz7z">gtirb</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jbzfdqpgsi">gtirb-capstone</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1n0cjaup07">gtirb-functions</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ecaug26728">gtk-tagged-streams</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=y98hs4339o">gtype.test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable GTYPE is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ourxnapr4">gtype</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable GTYPE is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3avtbo0kkh">gute</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jci2cd6j2">halftone</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vpcw0qdrb">hdf5-cffi.test</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kjyacomol">hdf5-cffi.examples</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x1422h8mwa">hdf5-cffi</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rjztsye0j">helambdap</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +MONTHS+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=b4fdds55ae">hemlock.tty</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1939ohpump">hemlock.qt</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ib7gs7y1c">hemlock.clx</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=49hh9lh0sn">hemlock.base</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wy392vdm2q">hh-aws</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ane2aesozx">horner</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mclbf96zz">http-body-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=141g1b0osz">http-body</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>9</td><td>24</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=900bjogkcm">hu.dwim.asdf.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dl10qqizi">hu.dwim.bluez</a> <span class="note">COMMON-LISP:FILE-ERROR : Filesystem error with pathname #P&quot;/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/hu.dwim.bluez-quicklisp-f3ebd960-git/c2ffi-spec/bluez.x86_64-apple-darwin9.spec&quot;.
Either
 1) the file does not exist, or
 2) we are not allowed to access the file, or
 3) the pathname points to a broken symbolic link.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ewdw26fg6s">hu.dwim.common.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qp1z0bgoa">hu.dwim.common-lisp.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dxqqjtcpzh">hu.dwim.computed-class.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x11f42f661&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qkpjjbqo9">hu.dwim.computed-class.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=c7w4qendxc">hu.dwim.computed-class+hu.dwim.logger</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x124037d61&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15tt7hh6cv">hu.dwim.debug.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12725p76xc">hu.dwim.def.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=beq3ul73xl">hu.dwim.def+hu.dwim.delico</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : core:instance-stamp was about to return a non-fixnum 0x10bb25f61</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ud3m8e6s8">hu.dwim.def+cl-l10n</a> <span class="note">EXT:STREAM-DECODING-ERROR : decoding error on stream
#&lt;IOFILE-STREAM #P&quot;/Users/karstenpoeck/lisp/fo... file-pos 1&gt;
(:EXTERNAL-FORMAT NIL):
  the octet sequence (190) cannot be decoded.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kmetpnv0il">hu.dwim.defclass-star.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17r5oghlqr">hu.dwim.delico</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : core:instance-stamp was about to return a non-fixnum 0x115749f61</span></td><td>0</td><td>2</td><td>2</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1oa9r9rcmy">hu.dwim.graphviz.test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libgvc.so&quot; &quot;libgvc.so.4&quot; &quot;libgvc32.so.4&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wo4s7hyj7">hu.dwim.graphviz.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mggdi9p0t">hu.dwim.graphviz</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libgvc.so&quot; &quot;libgvc.so.4&quot; &quot;libgvc32.so.4&quot;)</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rhnlbijq6">hu.dwim.logger.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12276c101&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1x6oy553qz">hu.dwim.logger.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14tqy8wfjj">hu.dwim.logger+swank</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12d00b901&gt;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kd83xur6f">hu.dwim.logger+iolib</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1oenpkxpz4">hu.dwim.logger</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12eb9e4a1&gt;</span></td><td>0</td><td>22</td><td>7</td><td>8</td><td>41</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=y8rk0mm3my">hu.dwim.partial-eval.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x1299d6ac1&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wldrir2td">hu.dwim.partial-eval.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=eq2ea8luex">hu.dwim.partial-eval</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12d7ab551&gt;</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nc4vo63rtj">hu.dwim.perec.test</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=b1xc046crn">hu.dwim.perec.sqlite.test</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jczlagxrg">hu.dwim.perec.sqlite</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pp3vnwh96">hu.dwim.perec.postgresql.test</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bzoy536tt8">hu.dwim.perec.postgresql</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jxvjpa9wle">hu.dwim.perec.oracle.test</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12xq4y6mlr">hu.dwim.perec.oracle</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=q5wdq7zmqh">hu.dwim.perec.documentation</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xqtyvlfmf5">hu.dwim.perec.all.test</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d2w25rjx15">hu.dwim.perec.all</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kfdkpax562">hu.dwim.perec+swank</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19vnfe0xut">hu.dwim.perec+iolib</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14umdcfikx">hu.dwim.perec+hu.dwim.quasi-quote.xml</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d5dopo2nh">hu.dwim.perec</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=faxlbnpx3f">hu.dwim.presentation+hu.dwim.web-server</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t8yu9yi26">hu.dwim.presentation+hu.dwim.stefil</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bboeev6v3">hu.dwim.presentation+cl-typesetting</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ukd0fitsh8">hu.dwim.presentation+cl-graph+cl-typesetting</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xf15uhrnt">hu.dwim.presentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>10</td><td>10</td><td>18</td><td>18</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wz5hpnz6o">hu.dwim.quasi-quote.xml+hu.dwim.quasi-quote.js</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2qzwto4rxm">hu.dwim.quasi-quote.test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mcxu596fsg">hu.dwim.quasi-quote.js</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=e97puc0bn5">hu.dwim.quasi-quote.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=m675vpxl9b">hu.dwim.rdbms.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12d0953c1&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vn4qys5xd">hu.dwim.rdbms.sqlite.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12a74f7c1&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14flzofwaq">hu.dwim.rdbms.sqlite</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x13b628581&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fpl0pg2mba">hu.dwim.rdbms.postgresql.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x15a1cdd41&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=feeh1xr69n">hu.dwim.rdbms.postgresql</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x14aee7551&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dqqc21q6s">hu.dwim.rdbms.oracle.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x125a73281&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=112varzw7v">hu.dwim.rdbms.oracle</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x130158381&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nf6bjdigh">hu.dwim.rdbms.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=we0flb791f">hu.dwim.rdbms.all.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12fe2cdc1&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mgcrm5xak9">hu.dwim.rdbms.all</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x133b8cba1&gt;</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fzis99lrr">hu.dwim.rdbms</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x136ac9c41&gt;</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>10</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qzmv0m0muq">hu.dwim.reiterate+hu.dwim.logger</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12fb8ea01&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1q3vqd06m4">hu.dwim.serializer.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cn27hjsyu">hu.dwim.syntax-sugar.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  c is not of type LIST.</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9xo4q655k2">hu.dwim.syntax-sugar.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1agfyjuzjc">hu.dwim.uri.test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8a10p5vvwg">hu.dwim.uri</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bmcmppi5k1">hu.dwim.util.test</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>6</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cya40gwgz">hu.dwim.util.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=iyqxmb9kib">hu.dwim.util+iolib</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=58iq88golh">hu.dwim.web-server.websocket</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=139d97esuu">hu.dwim.web-server.test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sqf62dc2ba">hu.dwim.web-server.documentation</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=50otazyxqb">hu.dwim.web-server.application.test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=a2z56ebriw">hu.dwim.web-server.application+hu.dwim.perec</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gdn07nb7ra">hu.dwim.web-server.application</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=399gm3trmk">hu.dwim.web-server+swank</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9y1kssj3p5">hu.dwim.web-server</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=l3t1yaujzq">hunchentoot-auth</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9hs61pglr0">hyperluminal-mem-test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1km4os7y6a">hyperluminal-mem</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e5v177cc3">hyperobject</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qgcsphg9a">ia-hash-table.test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tizqzjcrdn">iclendar</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : No :DIRECT-SUPERCLASS argument was supplied for metaclass #&lt;The BUILT-IN-CLASS NULL&gt;.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=52vcf1af3w">inferior-shell</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>7</td><td>6</td><td>7</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wdao51nkz">infix-math</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vfcyvqjuh">injection-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15xfu4g5q2">injection</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mwef898y7y">inlined-generic-function.test</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Unknown initialization options (&#039;CLOS::LEAF-METHOD-P) for class #&lt;The STANDARD-CLASS INLINED-GENERIC-FUNCTION:INLINED-METHOD&gt;.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5zb1ofrive">inner-conditional-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EVAL-ALWAYS| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=eywaotnuz4">inner-conditional</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EVAL-ALWAYS| is unbound.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ktq92qbiwa">inotify</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=h31ygl0int">inquisitor-flexi-test</a> <span class="note">ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-NOT-BE-FIRST : A symbol token must not start with two package markers as in ::name.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jhxj4k0pu">inquisitor-flexi</a> <span class="note">ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-NOT-BE-FIRST : A symbol token must not start with two package markers as in ::name.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1k0uf2upgc">integral-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=181dog2cnb">integral</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5w0yv13z2i">integral-rest-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b4x1lx3mw">integral-rest</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=puceoigiok">iolib.tests</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib.tests from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.tests.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vz3hje6zi">iolib.grovel</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9o4xz449gn">iolib.examples</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib.examples from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.examples.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ju3co3ols">iolib.common-lisp</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=45fot35cim">iolib.base</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=t4irdnr1gv">iolib</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>0</td><td>27</td><td>12</td><td>17</td><td>38</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3ocopul811">irc-logger</a> <span class="note">CLEAVIR-CST-TO-AST:LAMBDA-CALL-FIRST-SYMBOL-NOT-LAMBDA : Lambda call form was used with the malformed lambda block
first argument instead of the symbol LAMBDA. The following
form was found:
CREATE-LOGGER</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nzbxxaib9">iterate-clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1x63x3xr11">jenkins.api</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  0 is not of type LIST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ko36jg2sby">jingoh.tester.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e9jbmrcm4">jingoh.tester</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=51ap7iup22">jingoh.reader.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ld3m00vnhe">jingoh.reader</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15o8b37rhj">jingoh.parallel.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vg3n6nou8e">jingoh.parallel</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mdy8yjeg3">jingoh.org.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wrk6ewxve">jingoh.org</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cckywrcdsd">jingoh.examiner.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ewek7414f">jingoh.examiner</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=spf562txbm">jingoh.documentizer.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=q8g6tx50rx">jingoh</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=du9yv2qfmd">jonathan-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wfixcz1eaj">jonathan</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>20</td><td>12</td><td>21</td><td>46</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g9xf39h5t">jose</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ftq19742e">jpeg-turbo</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-I/usr/local/include&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=oqf902x287">js-parser-tests</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x9ajnp9rv3">js-parser</a> </td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12v4mxs6y2">jwacs-tests</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=syqdn8dtwt">kenzo-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=oz4c3of10p">kenzo</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1uwq2d2edc">keystone</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6ctqbzvh8h">l-math</a> <span class="note">EXT:UNDEFINED-CLASS : Could not find the class SIMPLE-ARRAY.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=euzglu7241">t-lack-session-store-redis</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ddpfaopqkp">t-lack-session-store-dbi</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jayoqdq3wb">t-lack-request</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o38tk9jej">t-lack-middleware-session</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12eb40lt5f">t-lack-middleware-csrf</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jyxniyye8">t-lack</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19bdogwkpq">lack-session-store-redis</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kyolashqc">lack-session-store-dbi</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1sz6zmpfdm">lack-request</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>8</td><td>22</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=175eizhe6x">lack-middleware-session</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=e0wvkf9u1d">lack-middleware-csrf</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=h066mthtt5">lastfm</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Filesystem error with pathname #P&quot;/Users/karstenpoeck/.config/.lastfmrc&quot;.
  Either
   1) the file does not exist, or
   2) we are not allowed to access the file, or
   3) the pathname points to a broken symbolic link.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lwt854mf9">leveldb</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBLEVELDB).
  NIL</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=22fbgcppu7">lfarm-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1iw31l935x">lfarm-ssl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fu3qhjkco">lfarm-server</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hk2svxepw2">lfarm-launcher</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1aqmks56st">lfarm-gss</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5ir97h86n9">lfarm-common</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>7</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6hmhucq22y">lfarm-client</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ffk2qctbx3">lfarm-admin</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s755uj5dar">lila</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-MOP&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i496wcw4y">lime-test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=168ivv0y4f">linear-programming-glpk</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libglpk&quot; &quot;libglpk.so.40&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=erc1fkso4t">linedit</a> <span class="note">ECLECTOR.READER:UNKNOWN-CHARACTER-NAME : Unrecognized character name: &quot;^F&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1gvljj1uzv">linux-packaging-tests</a> <span class="note">QL-HTTP:TOO-MANY-REDIRECTS : T,oo ,man,y r,edi,rec,ts ,(10) for #&lt;URL &quot;http://beta.quicklisp.org/archive/linux-packaging/2020-12-20/linux-packaging-20201220-git.tgz&quot;&gt;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=g9i1me2y62">linux-packaging</a> <span class="note">QL-HTTP:TOO-MANY-REDIRECTS : T,oo ,man,y r,edi,rec,ts ,(10) for #&lt;URL &quot;http://beta.quicklisp.org/archive/linux-packaging/2020-12-20/linux-packaging-20201220-git.tgz&quot;&gt;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nbfw7b7ez">lionchat</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jafzccucw">lisp-binary-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  When calling (FLET TRANSFORM-KEYWORDS) the bad keyword argument :FAIL was passed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9d8h4z7i6l">lisp-executable-tests</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hpdv1xa5l">zmq-examples</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not find package with (nick)name: ZMQ-EXAMPLES</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6y4a4r881t">lispbuilder-sdl-vecto-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ibeqd8vxry">lispbuilder-sdl-vecto</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=z9lqjne3ap">lispbuilder-sdl-ttf-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lqn79z08i9">lispbuilder-sdl-ttf-cffi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rwvj8bgoc">lispbuilder-sdl-ttf</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=167j0205jx">lispbuilder-sdl-mixer-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mp1jo7kmg">lispbuilder-sdl-mixer-cffi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=185u1px53v">lispbuilder-sdl-mixer</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>7</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vi1an83jo">lispbuilder-sdl-image-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11q4x5gozl">lispbuilder-sdl-image-cffi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tyvd3cfslp">lispbuilder-sdl-image</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>7</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hevitttwmk">lispbuilder-sdl-gfx-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xfqdx01ov">lispbuilder-sdl-gfx-cffi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wxlqfn5xj">lispbuilder-sdl-gfx</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gcee1tzswg">lispbuilder-sdl-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p8lphm1kt">lispbuilder-sdl-cl-vectors-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=uwr09dmto3">lispbuilder-sdl-cl-vectors</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j33zlbhx5i">lispbuilder-sdl-cffi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>0</td><td>23</td><td>4</td><td>5</td><td>28</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=odot059ho3">lispbuilder-sdl-base</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>5</td><td>27</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dr30uziba9">lispbuilder-sdl</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>5</td><td>26</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1f4jpbaohh">lispbuilder-regex</a> </td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1r1g0gui5r">lispbuilder-opengl-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=fukan1tt05">lispbuilder-net-cffi</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (NET).
  NIL</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8eg6xzdxxt">lispbuilder-net</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (NET).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12cdjbs14n">lispbuilder-lexer</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dlp7cas74">cocoahelper</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;cocoahelper&quot;) (:DEFAULT &quot;cocoahelper&quot;))</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vmeeknp6rn">lispcord</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=n7qb9xvbad">example-bot</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ll0oa891i">list-named-class</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1se0sbgbnv">litterae</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libyaml.dylib&quot; &quot;libyaml-0.2.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17zav2b716">lla</a> <span class="note">ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-NOT-BE-FIRST : A symbol token must not start with two package markers as in ::name.</span></td><td>0</td><td>1</td><td>1</td><td>5</td><td>9</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=uqzelpzo19">lmdb</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;FOO-RANDOM&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1f8w8dhnrt">log4slime</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13z820sutq">log4cl-examples</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qegev6oiuh">log4cl</a> </td><td>0</td><td>18</td><td>9</td><td>15</td><td>39</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yjcfv7kjim">lowlight.tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=28zgr8cli4">lowlight.old</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cuxbirs13">lowlight.doc</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=aim26m6ky7">lowlight</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qc78p7c05l">lucerne-utweet</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>4</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o26a678uj">lucerne-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>4</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10oans7l3j">lucerne-hello-world</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=iidk1gzic5">lucerne-auth</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>4</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1aedseitox">lucerne</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>2</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1gf0vm5n4x">macro-html</a> <span class="note">eclector.reader:package-does-not-exist : Package named &quot;[&quot; does not exist.</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18ofiqm7sc">magicffi</a> <span class="manual-note">ffi-grovel</span>, <span class="note">CFFI-GROVEL:GROVEL-ERROR : Subprocess with command (&quot;cc&quot; &quot;-o&quot; &quot;/Users/karstenpoeck/lisp/fork... &quot;-c&quot; &quot;-I/usr/include&quot; &quot;-I/usr/local/include&quot; &quot;-m64&quot; &quot;-I&quot; &quot;/opt/local/include/&quot; &quot;-fPIC&quot; &quot;-I/Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cffi_0.23.0/&quot; &quot;/Users/karstenpoeck/lisp/fork...
 exited with error code 256</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=r96ibk6vwj">magicl-transcendental</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=100kbacp91">magicl-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nqknoiwp1m">magicl-examples</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sp3zpdunfh">magicl</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nau8fvlbw8">maiden-weather</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d5jba89oq9">maiden-vote</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bw27cuh99u">maiden-urlinfo</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5puy7l76ow">maiden-twitter</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jtwp4s91j">maiden-trivia</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11or2v9l05">maiden-time</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=o1fw72893o">maiden-throttle</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15oxwiygtk">maiden-talk</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=159h2nn68h">maiden-storage</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1c0xbna5pd">maiden-silly</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x43hq7owlx">maiden-serialize</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bldba21a0">maiden-relay</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=straes92rg">maiden-permissions</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ogpn0exfz">maiden-notify</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pdwb8qg2qn">maiden-networking</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=9j0i5huqlk">maiden-medals</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11ovx30r4f">maiden-markov</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1oj2oatq2e">maiden-lookup</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=iux25nht1k">maiden-location</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tv3a71krqd">maiden-lichat</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7e6i7t92xb">maiden-lastfm</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1232ld07ic">maiden-irc</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18356d0ynb">maiden-help</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11s0bv7m10">maiden-emoticon</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ty6yefxfbf">maiden-dictionary</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14qoiggtbu">maiden-crimes</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nuhywyabqh">maiden-counter</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g9ud1y87a">maiden-core-manager</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14j39mpcpk">maiden-commands</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10n669vswy">maiden-client-entities</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1s463o9ppb">maiden-chatlog</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1una3pnkhl">maiden-channel-relay</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qbcp3op0v">maiden-blocker</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bzvsc7ci35">maiden-api-access</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1y09y3m0bl">maiden-activatable</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tnk0c5fis">maiden-accounts</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pwouttavw9">maiden</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mivonj6s5">make-hash-tests</a> <span class="note">CORE:SIMPLE-READER-ERROR : Undefined reader macro for char &#039;#&#039; subchar &#039;&#039;&#039; in file tests.lisp line: (1573) column (35).</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1oh3kbbfs6">markup.test</a> <span class="note">ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-BE-ADJACENT : If a symbol token contains two package markers, they must be adjacent as in package::symbol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1opitc6t45">matrix-case.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=so15q1o3lw">scigraph</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  When calling (FLET TRANSFORM-KEYWORDS) the bad keyword argument :ABORT was passed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hwxfm8i25">clim-listener</a> </td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tfb4gij8ue">media-types</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2882vj2jbg">mel-base</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;NIL&quot;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1oraedgk5h">metacopy-with-contextl</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14oqnsmf4a">metatilities-test</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ggtrbh94c">metatilities</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>0</td><td>4</td><td>2</td><td>7</td><td>23</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10j3zr0t2g">method-combination-utilities</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  keyword list is not a proper list</span></td><td>0</td><td>3</td><td>2</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15bvmradml">method-hooks-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-STRUCTURE-MISMATCH-ERROR : Could not destructure (&quot;echo ~a&quot;) according to
((LAMBDA-CST LAMBDA-LIST-CST . BODY-CST) . ARGS-CST) because
#&lt;ATOM-CST raw: &quot;echo ~a&quot; @0x12ebab4f1&gt; is not a CONS-CST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1h3nza3xz7">mexpr-tests</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1w480p7bh7">mgl-pax</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;FOO-RANDOM&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>5</td><td>9</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qv9z09m4v">micmac</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;FOO-RANDOM&quot; does not exist.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=z3dbabczgc">millet.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10brrcobqp">minheap-tests</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1eaqh40aae">minilem</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ujctyghtci">mito-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t7sbh8wum">mito-migration</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tqlmv8y1f">mito-core</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1b9zpeosrx">mito</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1arrzzopjv">lack-middleware-mito</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=aoo10ca5ly">mito-attachment</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lc500lkb3">mito-auth</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ohbr6b275">moira</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1va2g95w1z">monomyth</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o6a0qi613">montezuma-indexfiles</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-INT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17z89wjnjf">mop-utils</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Error: Name conflict for USE-PACKAGE of [CLOSER-MOP] by package[MOP-UTILS]
   - conflicting symbols:  &quot;STANDARD-GENERIC-FUNCTION&quot; &quot;DEFGENERIC&quot; &quot;DEFMETHOD&quot;</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=j9k119z0eg">mtlisp</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=u45k6ghove">multiposter-twitter</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-MOP&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=m31uf0xs4s">multiposter-tumblr</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-MOP&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tnsarzzkr">multiposter-studio</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-MOP&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fyxx6ul27">multiposter-mastodon</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-MOP&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=87ly1k3igf">multiposter-git</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-MOP&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ft1eunint">multiposter</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-MOP&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=869j8crqyh">multival-plist-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p7zaanezo">multival-plist</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>1</td><td>1</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g8oj6oa3r">napa-fft3</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Package error on package &quot;SB-EXT&quot;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11o5p46hh1">nbd</a> <span class="note">SB-BSD-SOCKETS:HOST-NOT-FOUND-ERROR : Name service error in &quot;get-host-by-name&quot;: +HOST-NOT-FOUND+ (Operation not permitted)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=41r4zf89fu">neural-classifier</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fve4zhw4y">nibbles</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>133</td><td>66</td><td>96</td><td>219</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15cy0ynvbf">nineveh</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xl9qrnmuh">ningle-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=41yvrzez9n">ningle</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>7</td><td>12</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4fhg73evgn">nodgui</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  ERROR during macroexpansion:
    -922337203685477581 is not of type LIST.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dswxi84av">nuclblog</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3cnz45jdm9">null-package.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11u5dzoeu3">numcl.test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable GTYPE is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=197gpzkwwz">numcl</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable GTYPE is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rz4ans1z0z">oclcl-test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bv4w80t0yz">oclcl-examples</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ayswswlrah">oclcl</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18amgvnw0k">ook</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +OOKS+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mhdsuhqgad">oook</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=oy1v6bpfve">openid-key-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wnir60qowx">openid-key</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17p4j7muyw">org-davep-dict</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1v60sp1034">org-davep-dictrepl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13d0a0236u">net.mfiano.lisp.origin.test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d2ppriur0">net.mfiano.lisp.origin</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1eqrgx1ene">orizuru-orm</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dkd9dj496a">overlord</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5px1ew4asn">packet-crafting</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1iin7yyuks">pal</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libSDL-1.2.so.0&quot; &quot;libSDL-1.2.so&quot;)</span></td><td>0</td><td>6</td><td>3</td><td>3</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5vf3pquemi">bermuda</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libSDL-1.2.so.0&quot; &quot;libSDL-1.2.so&quot;)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wohaep68t">test-paren6</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : This lisp implementation is not supported by the EXTERNAL-PROGRAM library.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qez2ho532w">parseltongue</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1j0env21q0">net.mfiano.lisp.patchwork</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=944jz4234d">patron</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  `WITHOUT-INTERRUPTS&#039; is not supported!</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ncvw8qs4q">perceptual-hashes</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=b8legy6hc9">periods-series</a> </td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xp2pfr831o">periods</a> </td><td>0</td><td>2</td><td>1</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=55zw8jp5gz">petalisp.type-inference</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12r33uipv0">petalisp.test-suite</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kjnysx6rqb">petalisp.scheduler</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rlfq8xbm7x">petalisp.native-backend</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=n6lpnq974z">petalisp.ir</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mjfplc1uef">petalisp.graphviz</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19grqiqwfy">petalisp.examples</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=e1i2t1yz4x">petalisp.core</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ofqclb0w8z">petalisp.api</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1j7xzx8vsq">petalisp</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=n57ecldaik">pettomato-indexed-priority-queue-tests</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-EXT&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qis3pykju">pg</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  No system dependent code to convert from client encoding to external format name</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7j2drjcxxm">pgloader</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (SYBDB).
  NIL</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1alzr1fu23">piggyback-parameters</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18b9pvsjwt">pileup</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12c666641&gt; where a CONS-CST is required.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=l3y4fsn1ku">pkg-doc</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2wnboxaf4d">plain-odbc</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (ODBC).
  NIL</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1kvp4i5aqt">planks</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Unsupported implementation: clasp</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1plyf62xdz">pngload.test</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bcnur4a6w">pngload</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qswbr00xm8">portable-threads</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Calling IMPORT - Got 0 arguments, but expected between 1 and 2</span></td><td>0</td><td>2</td><td>1</td><td>2</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rmazm1f1m">webactions</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1oewm4d7au">htmlgen</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>8</td><td>25</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14bt0hbui8">aserve</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>8</td><td>24</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yw9pqmy2n0">acl-compat</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>12</td><td>34</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nbntkzv3p1">postoffice</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qvt9amkrhk">pounds</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>2</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ziqhzt2omj">pp-toml-tests</a> <span class="note">ECLECTOR.READER:UNKNOWN-CHARACTER-NAME : Unrecognized character name: &quot;Form&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ghw2bqiy86">pp-toml</a> <span class="note">ECLECTOR.READER:UNKNOWN-CHARACTER-NAME : Unrecognized character name: &quot;Form&quot;</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1elkjiucgr">practical-cl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=avfdt6tfpp">pcl-url-function</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ihqweo6hv">pcl-shoutcast</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=up253vyweh">pcl-mp3-browser</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ygv0kzwszp">printv</a> <span class="note">COMMON-LISP:UNDEFINED-FUNCTION : The function MAKE-RECURSIVE-LOCK is undefined.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bouymy4xds">projectured.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12c98e661&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4tkaa63l4q">projectured.swank</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x1256cf701&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nuw499rq9">projectured.sdl.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x1334fd131&gt;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dx5c5atjab">projectured.sdl</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x11d900581&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qftpmbi7o7">projectured.projection</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12378f1a1&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1woe5gyja7">projectured.executable</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x12d4631e1&gt;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4lopwimo20">projectured.editor</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x123fe2441&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>7</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10t6f2igu1">projectured.document</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Cannot find ROOT-LOGGER in namespace #&lt;NAMESPACE LOGGER @0x119d4e041&gt;</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=i1452fvo80">prometheus.test.all</a> </td><td>5</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3hbrgxfr9e">prometheus.test</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p6vwut4sy">prometheus.pushgateway.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in method specializer (VALUE (EQL))</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3g87a5k25b">prometheus.pushgateway</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in method specializer (VALUE (EQL))</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15xx1fr0v7">prometheus.formats.text.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in method specializer (VALUE (EQL))</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nlq3l1rxca">prometheus.formats.text</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in method specializer (VALUE (EQL))</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>7</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=l197siz2e8">prometheus.exposers.hunchentoot.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in method specializer (VALUE (EQL))</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=grfa4baq6j">prometheus.exposers.hunchentoot</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in method specializer (VALUE (EQL))</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16xsy1faoj">prometheus.examples</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Syntax error in method specializer (VALUE (EQL))</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=r5yc63auo4">prometheus.collectors.sbcl.test</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-THREAD&quot; does not exist.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bkp5x9kxl">prometheus.collectors.sbcl</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-THREAD&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cvuzpmcn2p">prometheus.collectors.process.test</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1h7z9zyj2q">prompt-for.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=q70dt4kdwb">varint</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>3</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14yreinnvl">protobuf</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1n98u4jn9g">psychiq-test</a> </td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=oyymylq4bi">psychiq</a> </td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tehzymjzr">smokebase</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system smokebase from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/smokebase.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15yf0343oz">qwt</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qwt from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qwt.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ugqci4ypu">qtxmlpatterns</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtxmlpatterns from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtxmlpatterns.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1w1gx4zkag">qtxml</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtxml from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtxml.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17vgasciyh">qtwebkit</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtwebkit from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtwebkit.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bqcn8difk">qtuitools</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtuitools from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtuitools.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2a807sep9w">qttest</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qttest from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qttest.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1h84quz0oh">qtsvg</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtsvg from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtsvg.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2ow88q2s9v">qtsql</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtsql from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtsql.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1amm0tfe9t">qtscript</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtscript from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtscript.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14j19v4rxz">qtopengl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtopengl from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtopengl.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>4</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mk8z7w3t3">qtnetwork</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtnetwork from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtnetwork.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lm1xqelx6a">qthelp</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qthelp from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qthelp.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15lkkp59wt">qtgui</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtgui from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtgui.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>6</td><td>34</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bmwsvnnejh">qtdeclarative</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtdeclarative from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtdeclarative.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pk76m9doy">qtdbus</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtdbus from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtdbus.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zbxwju0dde">qtcore</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>6</td><td>34</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yym4hkuyhx">qt3support</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qt3support from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qt3support.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11w3w25rel">qt-libs</a> <span class="note">EXT:ASSERT-ERROR : The assertion (UIOP/UTILITY:LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>55</td><td>5</td><td>6</td><td>56</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1adm0sypqx">qsci</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qsci from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qsci.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1f8r70fwu5">qimageblitz</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qimageblitz from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qimageblitz.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1r2pzxqf64">phonon</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system phonon from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/phonon.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1uptx3jqbj">commonqt</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system commonqt from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/commonqt.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=z5vsfg9ryb">qtools-titter</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ylp6una3j3">qtools-opengl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1eqndepsat">qtools-melody</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e2nr3d4m0">qtools-helloworld</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtools-helloworld from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qtools-20200427-git/examples/helloworld/qtools-helloworld.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=as9vb1rigt">qtools-game</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8yqbaum50c">qtools-evaluator</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i9desu07n">qtools</a> <span class="note">EXT:ASSERT-ERROR : The assertion (UIOP/UTILITY:LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>6</td><td>55</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jl1eafe0m">q+</a> <span class="note">EXT:ASSERT-ERROR : The assertion (UIOP/UTILITY:LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=m8alw3f222">qtools-ui-svgtools</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bl2dt0jck6">qtools-ui-splitter</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lertfynm0h">qtools-ui-spellchecked-text-edit</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a4iorlq6s">qtools-ui-slider</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17m6suwrcp">qtools-ui-repl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wewjrprkj2">qtools-ui-progress-bar</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fwqgzilnd">qtools-ui-plot</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12gvf2q2vo">qtools-ui-placeholder-text-edit</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13f7u485l4">qtools-ui-panels</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7o1leqcrdf">qtools-ui-options</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zulxv9f6w1">qtools-ui-notification</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jluyoal1o">qtools-ui-listing</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ncpw1zh2ne">qtools-ui-layout</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>17</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xju3yc2b1">qtools-ui-keychord-editor</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a9fmychdr">qtools-ui-imagetools</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qimageblitz from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qimageblitz.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kz09fnkrqr">qtools-ui-helpers</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>13</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1r7qd1uzw1">qtools-ui-flow-layout</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=z0zk4gvckd">qtools-ui-fixed-qtextedit</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=cedpywoq3x">qtools-ui-executable</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d53wlsi9hf">qtools-ui-drag-and-drop</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=oq91hul4ah">qtools-ui-dictionary</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qorafq91z">qtools-ui-dialog</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1upbx57doi">qtools-ui-debugger</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=azyy6m2plt">qtools-ui-container</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>8</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1onvdx5uiz">qtools-ui-compass</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mm1dlyw6i">qtools-ui-color-triangle</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14mqyztil1">qtools-ui-color-sliders</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=138rjz82gb">qtools-ui-color-picker</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1711bxqewg">qtools-ui-color-history</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=afp32ch41x">qtools-ui-cell</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12g11ij3ox">qtools-ui-bytearray</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ax7g0x2di">qtools-ui-base</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>23</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wt74yviic1">qtools-ui-auto-resizing-textedit</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=aw0plxucyv">qtools-ui</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hpi6azp7z">quantile-estimator.test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6q75s5p5p7">queen</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=i7iyfwuj9c">query-fs</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBFUSE).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14p7h5krph">queues.priority-queue</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Structure definition for NODE cannot have :NAMED without :TYPE.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8flyr3mscu">queues.priority-cqueue</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Structure definition for NODE cannot have :NAMED without :TYPE.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5l5t5ftzrt">quickutil-utilities-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rcfb3vx7v4">quickutil-server</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>3</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dfj7tv8hi">quilc-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=zl68phuwva">quilc</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bo97abvko0">cl-quil-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=122ossyt4p">cl-quil-benchmarking</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ta745auca">cl-quil</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=e5jkmr3kye">boondoggle-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=93bhhynvtr">boondoggle</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5zvzw890tm">qvm-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vugp581di">qvm-examples</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=58ivpzalct">qvm-benchmarks</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=m7muen3u5t">qvm-app-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=191oxg8du6">qvm-app-ng-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ofva651n6">qvm-app-ng</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1y0ds8kgzn">qvm-app</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=tiq38vm5fs">qvm</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  WITH-ARRAY-POINTERS unsupported on clasp</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=st8knli2fz">racer</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6l25heuyxl">lracer</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Cannot modify value of constant +NRQL-SYMBOLS+</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rjz8wru1g">random-sample</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6m59vsp0r0">random-state-viewer</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system qtcore from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/qt-libs-20201220-git/systems/qtcore.asd: The assertion (LENGTH=N-P ASDF/ACTION::FILES 1) failed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1i2fg0kdov">rcl</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Can&#039;t find library libR.dylib in /Library/Frameworks/R.framework/Resources/lib/, verify settings in config.lisp</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18veyp6ob1">read-as-string.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yl68hlgyuv">regex</a> </td><td>0</td><td>2</td><td>2</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15p8lajqhk">scrutiny-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x128ed8a01&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=owffrfsdvi">scrutiny</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12504f581&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vf7f7v0rsa">rte-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system rte-test from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/regular-type-expression-export-to-quicklisp-502a46e2-git/rte/rte-test.asd: Encountered #&lt;ATOM-CST raw: NIL @0x124f7e881&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=bt3yjqmgx7">rte-regexp-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x1267dd6d1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ox38vvbnie">rte-regexp</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x1266d0ee1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dg7zy5uvdx">rte</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x126274791&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1s686dw0cp">research</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system rte-test from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/regular-type-expression-export-to-quicklisp-502a46e2-git/rte/rte-test.asd: Encountered #&lt;ATOM-CST raw: NIL @0x121c8d941&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ap3hrxers6">ndfa-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12fdef5f1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cm31p0c42">ndfa</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12fc3e581&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1voa037q5l">lisp-types-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12c237941&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=132lr5258a">lisp-types-analysis</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x129d5fc41&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8br1zfv2z6">lisp-types</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x131ab4ac1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=142b8l6ku4">dispatch-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12e3e5931&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=10gwhli818">dispatch</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x1270e55c1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ul2zenh6n6">cl-robdd-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x128855b81&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=r3nfr9itty">cl-robdd-analysis-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12edea581&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=x066y74izg">cl-robdd-analysis</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x126bc9a01&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=f5p1tl1jii">cl-robdd</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12c401ac1&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7m9p936oda">adjuvant-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12ad84101&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tt4dh3k7p">adjuvant</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x126da7d51&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=k2chspk0y0">2d-array-test</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x12d493441&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1emphhm13k">2d-array</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not find package with (nick)name: 2D-ARRAY</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1w4rcsdddn">replic-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cwpgworsd">replic</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bv2sd6op2">resignal-bind.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pmcya1n18x">restful-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15mr3jv65e">restful</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xsvwdaa9by">roan</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=za0o44e3qg">rock-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s11zwx3ytt">rpm</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wxh59bjq4s">rt-events.examples</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  When calling (FLET TRANSFORM-KEYWORDS) the bad keyword argument :TIMEOUT was passed</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mizi4ntd2f">rt-events</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  When calling (FLET TRANSFORM-KEYWORDS) the bad keyword argument :TIMEOUT was passed</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1x9bh6u50b">rtg-math.vari</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ut01njrdv0">rucksack-test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Unsupported implementation: clasp</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1we5qwqd4m">rucksack</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Unsupported implementation: clasp</span></td><td>0</td><td>1</td><td>1</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=p8mkt6eqiy">rutilsx</a> </td><td>0</td><td>2</td><td>2</td><td>3</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fdkueaskt">rutils-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=420vv5goal">rutils</a> </td><td>0</td><td>9</td><td>6</td><td>9</td><td>16</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wuxf89tiq">ryeboy</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system ryeboy from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/ryeboy-20201016-git/ryeboy.asd: Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18pjbej12x">sb-fastcgi</a> <span class="note">QUICKLISP-CLIENT:SYSTEM-NOT-FOUND : System &quot;sb-alien&quot; not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1quguxphqn">sb-vector-io</a> <span class="note">ECLECTOR.READER:PACKAGE-DOES-NOT-EXIST : Package named &quot;SB-SYS&quot; does not exist.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2q9ezaqtci">sc-extensions</a> <span class="note">CONCRETE-SYNTAX-TREE:CONS-CST-REQUIRED : Encountered #&lt;ATOM-CST raw: NIL @0x127eaa221&gt; where a CONS-CST is required.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=kud0q9ijin">scribble</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  ERROR during macroexpansion:
    too many arguments</span></td><td>0</td><td>1</td><td>1</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t5ada0r9i">scriptl-util</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system scriptl-util from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/scriptl-20180228-git/scriptl-util.asd: Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rvudl49dx">scriptl-examples</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system scriptl-examples from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/scriptl-20180228-git/scriptl-examples.asd: Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=i6cjz6274c">scriptl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system iolib from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/iolib-v0.8.3/iolib.asd: ERROR during macroexpansion:
  Your CL implementation isn&#039;t supported.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p7jq5jez0">software-evolution-library</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=s24h8wuyhf">semantic-spinneret</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=113mhgpjww">serapeum</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>16</td><td>5</td><td>5</td><td>17</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12zf329i3b">series</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Lambda call form was used with the malformed lambda block
  first argument instead of the symbol LAMBDA. The following
  form was found:
  *OPTIMIZE-SERIES-EXPRESSIONS*</span></td><td>0</td><td>10</td><td>2</td><td>3</td><td>11</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1q6r2k7p5g">sexml-objects</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Unknown initialization arguments for #&lt;The STANDARD-CLASS CL-ATTRIBS:ATTRIBUTED-EFFECTIVE-SLOT&gt;: (:ALLOCATION-CLASS
                                                                                                  :CLASS)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1r1k8gcpsa">net.mfiano.lisp.shadow</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1fdv6uhvhu">sheeple</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>3</td><td>2</td><td>2</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nsq2glebe">shellpool</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system shellpool from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/shellpool-20200925-git/shellpool.asd: 

Error: Shellpool has not yet been ported to this Lisp; patches welcome.

</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13imnwliti">should-test</a> </td><td>1</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ss8yqych4">simple-currency</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tmj3c9og6">simple-neural-network</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=pg4ofwgess">sip-hash</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5wxychagw5">sketch-examples</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;SDL2_image&quot;) (:DEFAULT &quot;libSDL2_image&quot;))</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6xf43uimvp">sketch</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   ((:FRAMEWORK &quot;SDL2_image&quot;) (:DEFAULT &quot;libSDL2_image&quot;))</span></td><td>2</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1qqdfah985">skitter.glop</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (BRIDGE).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=13amw67jf1">slack-client-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ei6uu6wa3">slack-client</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=sabod6pliv">smackjack-demo</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system smackjack from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/smackjack-20180228-git/smackjack.asd: Too few arguments supplied to a macro or a destructuring-bind form:
(:FILE)</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ji9r2akohj">smackjack</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system smackjack from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/smackjack-20180228-git/smackjack.asd: Too few arguments supplied to a macro or a destructuring-bind form:
(:FILE)</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ienr9z0pag">snappy</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=8f37eub2sp">snmp-ui</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Calling IMPORT - Got 0 arguments, but expected between 1 and 2</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qgdjv9r9lw">snmp-test</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Calling IMPORT - Got 0 arguments, but expected between 1 and 2</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=lbj7balbgu">snmp-server</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Calling IMPORT - Got 0 arguments, but expected between 1 and 2</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11c3zeqgzp">snmp</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Calling IMPORT - Got 0 arguments, but expected between 1 and 2</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1n81tnjtgh">specialization-store-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1oyd3tdlkb">specialization-store</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=axiscpx47s">spell</a> <span class="note">ECLECTOR.READER:READ-TIME-EVALUATION-ERROR : Read-time evaluation of expression (LOAD-DICTIONARY
                                    (ASDF/SYSTEM:SYSTEM-RELATIVE-PATHNAME
                                     :SPELL
                                     &quot;english.txt&quot;)) signaled ECLECTOR.READER:TWO-PACKAGE-MARKERS-MUST-NOT-BE-FIRST: A symbol token must not start with two package markers as in ::name.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7hkb8zo0i8">spinneret</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>4</td><td>1</td><td>1</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1s2vi1zu14">staple-server</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mxbplvfrxu">staple-restructured-text</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xmprx7m4q">staple-markless</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g7u2lcblf">staple-markdown</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=g11v2xkjuh">staple-code-parser</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=i5fi6dz76s">staple</a> <span class="note">ECLECTOR.READER:MULTIPLE-OBJECTS-FOLLOWING-CONSING-DOT : Only a single object can follow a consing dot.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rl8qr7u1dt">static-dispatch</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Cannot export the symbol CLOSER-MOP:STANDARD-GENERIC-FUNCTION from #&lt;PACKAGE CLOSER-ENVIRONMENTS&gt;,
  because there is already a symbol with the same name
  in the package.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d0fdi9hje">stefil+</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=rvcz7t8arq">stl</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1g6r7banla">stmx.test</a> </td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1htogk0a22">stmx</a> </td><td>1</td><td>0</td><td>0</td><td>2</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1l0zh8lq52">structure-ext.make-instance.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1jt0cwka9x">structure-ext.left-arrow-accessors.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1h1n70i1e5">structure-ext.as-class.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vquaq33okd">stumpwm-tests</a> <span class="note">QUICKLISP-CLIENT:SYSTEM-NOT-FOUND : System &quot;sb-posix&quot; not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=un3yhbv24y">stumpwm</a> <span class="note">QUICKLISP-CLIENT:SYSTEM-NOT-FOUND : System &quot;sb-posix&quot; not found</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=18467d32cu">submarine</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Error: Name conflict for USE-PACKAGE of [CLOSER-MOP] by package[MOP-UTILS]
   - conflicting symbols:  &quot;STANDARD-GENERIC-FUNCTION&quot; &quot;DEFGENERIC&quot; &quot;DEFMETHOD&quot;</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=nomav1586s">window</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a0pghjgip">text-subsystem-generate-font</a> <span class="note">EXT:UNDEFINED-CLASS : Could not find the class FOREIGN-WRAPPER.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1gb6kh94xm">text-subsystem</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=njzi1g0bwh">sucle-test</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vwqo8ogm8">sucle</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=i1nd5xiq50">ncurses-clone-for-lem</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=hoibsq9k97">lem-opengl</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ltgradnly7">control</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3i4toelyno">application</a> <span class="note">CFFI::UNDEFINED-FOREIGN-TYPE-ERROR : Unknown CFFI type (:STRUCT %GLFW::CURSOR)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1mvejwt40s">sxql-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qugx0fvxz5">sxql</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>9</td><td>4</td><td>11</td><td>19</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1vcjbkym9s">sxql-composer</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=15kdhk3mda">tagger</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Don&#039;t know how to represent -infinity.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1659agh342">talcl</a> <span class="note">PURI:URI-PARSE-ERROR : Parse error:URI &quot;file:// /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/buildnode-20170403-git/src/xhtml1-transitional.dtd&quot; contains illegal character #\NUL at position 7.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=3sxmf3ge83">teddy</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dpgsuzh65">teepeedee2-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  -922337203685477581 is not of type LIST.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=m52ezfamqz">teepeedee2</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  -922337203685477581 is not of type LIST.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ug16mvvzf">template-function-tests</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jf8z1kq2e4">template-function</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1cwrwc2tn0">ten.i18n.cl-locale</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=agib75a6ct">test-utils</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  (FDEFINITION) is an illegal SETF form.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=2btbas9j75">thread.comm.rendezvous.test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bzg2elc0m">thread.comm.rendezvous</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT| is unbound.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=d86xp6zaf8">tinaa-test</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=w6ve50pvfq">tinaa</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=b9c6hg6dwg">toadstool-tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  This is not implemented for your lisp, sorry. You may try to continue, but...</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ngw64ttp2">transparent-wrap</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  (ECLECTOR.READER:UNQUOTE X) is not of type (OR STRING SYMBOL CHARACTER).</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14a1ls7p1j">trestrul.test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:

  NIL is invalid.
  HINT: NULL?</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=krhnc36ngd">trivial-continuation</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1a2mpsnjo4">trivial-json-codec</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=xrp44x3lsv">trivial-monitored-thread</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jqqieqnsm5">trivial-nntp</a> <span class="note">ECLECTOR.READER:UNKNOWN-CHARACTER-NAME : Unrecognized character name: &quot;period&quot;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1tf0ln5vp1">trivial-object-lock</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=jniq96uwvw">trivial-octet-streams</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Invalid function name: (ERROR &quot;octet streams not supported in this implementation&quot;)</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bp7ygaqwe">trivial-pooled-database</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=11c9havttm">trivial-raw-io</a> <span class="note">CORE:SIMPLE-READER-ERROR : Undefined reader macro for char &#039;#&#039; subchar &#039;$&#039; in file raw-io.lisp line: (31) column (30).</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7uerifw9oq">trivial-sockets</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system trivial-sockets from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/trivial-sockets-20190107-git/trivial-sockets.asd: keyword list is not a proper list</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1hfc79wr0d">trivial-ssh-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBSSH2).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1t7e3dk4b3">trivial-ssh-libssh2</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBSSH2).
  NIL</span></td><td>0</td><td>2</td><td>1</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=qtwb5ixhw2">trivial-ssh</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load foreign library (LIBSSH2).
  NIL</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=4g7f1phiya">trivial-timer</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1nsj2jv7oh">trivial-ws-test</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19rbq8nizb">trivial-ws-client</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=gv71uxstzw">trivialib.bdd.test</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=c7yc3b18z5">trivialib.bdd</a> <span class="note">COMMON-LISP:SIMPLE-ERROR : Your Lisp does not support weak value hash-tables.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=12kz3w1zop">trucler-native-test</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  No applicable method for DESCRIBE-VARIABLE with arguments
   (#&lt;TRUCLER-NATIVE:CLIENT&gt; #&lt;VARIABLE-IGNORE E IGNORABLE @0x13312da41&gt; A)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1badpvqo5w">type-i.test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14icpca7tl">ucw-core</a> </td><td>0</td><td>5</td><td>1</td><td>1</td><td>5</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=uyn551dmxt">ucw</a> </td><td>1</td><td>0</td><td>0</td><td>1</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=778feoqx0t">uffi-tests</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vaawwi3nxy">uffi</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component &quot;uffi&quot; not found</span></td><td>0</td><td>36</td><td>19</td><td>22</td><td>40</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1lljzkv539">net.mfiano.lisp.umbra</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  No attempt has been made to determine if this implementation supports the Metaobject Protocol.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5ayy2q3b7u">umlisp-tests</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1txg5gloxd">umlisp</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wljayd3m0n">umlisp-orf</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1u7ro24fn9">uncursed-examples</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Last argument of APPLY is not a list/frame/activation-frame - passed #&lt;CLOSURE-WITH-SLOTS@0x10dba1580  MAKE-HASH-TABLE :type cclasp  lambda-list: (&amp;KEY (TEST (FUNCTION EQL)) (SIZE 0) (REHASH-SIZE 2) (REHASH-THRESHOLD 0.7) WEAKNESS DEBUG THREAD-SAFE) :fptr 0x1103fdf60&gt;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1o95x03kgc">uncursed</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Last argument of APPLY is not a list/frame/activation-frame - passed #&lt;CLOSURE-WITH-SLOTS@0x1114969e0  MAKE-HASH-TABLE :type cclasp  lambda-list: (&amp;KEY (TEST (FUNCTION EQL)) (SIZE 0) (REHASH-SIZE 2) (REHASH-THRESHOLD 0.7) WEAKNESS DEBUG THREAD-SAFE) :fptr 0x113cf6f60&gt;</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1n326tzq3j">uri-template.test</a> <span class="note">CORE:SIMPLE-READER-ERROR : Undefined reader macro for char &#039;#&#039; subchar &#039;U&#039; in file uri-template-test.lisp line: (35) column (18).</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1og5tm3csb">utilities.binary-dump</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>1</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pcokdz20o">validate-list</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=okid0wtgmm">varjo.tests</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1bnweve2sm">varjo</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  The variable VARJO.INTERNALS:: is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ubzslllc00">vernacular</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=148h57wriz">verrazano</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : The symbol TYPE-OF is bound to an ordinary function and is not a valid name for a generic function</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1pwcc53w97">vom-json</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1rmeeop7vc">weblocks-yui</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=546jz5efv5">weblocks-yarek</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yih7akxafo">weblocks-util</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>5</td><td>18</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=wd6ro50t5p">weblocks-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>3</td><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=19p5hltwki">weblocks-s11</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=7e2f1lsc00">weblocks-demo-popover</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1dcm2hh7zc">weblocks</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>5</td><td>11</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=whdv2lo4j3">weblocks-demo</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1ep3kctxrr">weblocks-clsql-demo</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=r6gdplq50o">simple-blog</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=mo29pqjp35">weblocks-prototype-js</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>3</td><td>0</td><td>0</td><td>2</td><td>2</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=6q2btowhdn">weblocks-stores</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>5</td><td>17</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=dx0k383t2y">weblocks-store-test</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16c0xczatf">weblocks-prevalence</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16pl9flwol">weblocks-perec</a> <span class="note">EXT:ASSERT-ERROR : The assertion (&lt;= (LENGTH METACOPY-SYSTEM::PATHS) 1) failed</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=vhmu7tauu3">weblocks-montezuma</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p5x30sl2b">weblocks-memory</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>4</td><td>6</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=16r0k5n0ag">weblocks-custom</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>4</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=96rnoub1zt">weblocks-clsql</a> <span class="note">ASDF/FIND-COMPONENT:MISSING-COMPONENT : Component UFFI not found</span></td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1s31ql80fg">weblocks-tree-widget</a> <span class="note">CORE:SIMPLE-PACKAGE-ERROR : Cannot export the symbol #:ROOT from #&lt;PACKAGE METABANG.UTILITIES&gt;,
because there is already a symbol with the same name
in the package.</span></td><td>2</td><td>0</td><td>0</td><td>4</td><td>4</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1wz6v5lugf">weblocks-utils</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>3</td><td>0</td><td>0</td><td>3</td><td>3</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1d1kruoqjk">weft</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1xu1inio6a">winlock</a> <span class="note">CLEAVIR-CST-TO-AST:MACROEXPANSION-ERROR : ERROR during macroexpansion:
  Symbol QUASIQUOTE is unbound in namespace PATTERN</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=suuy312cww">with-c-syntax-test</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=5o0r4f7uup">woo-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@DOC| is unbound.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=n0phvmpaxd">wookie</a> <span class="manual-note">ffi</span>, <span class="note">CFFI:LOAD-FOREIGN-LIBRARY-ERROR : Unable to load any of the alternatives:
   (&quot;libuv.dylib&quot;)</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1p0w2xf37k">wuwei</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system acl-compat from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/portableaserve-20190813-git/acl-compat/acl-compat.asd: The acl-compat library is not yet supported on this lisp implementation.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=ct0x4a2dks">xcat</a> </td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=14v5ud9vhj">xecto</a> <span class="note">QUICKLISP-CLIENT:SYSTEM-NOT-FOUND : System &quot;sb-queue&quot; not found</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=yh3fttbyxo">zacl</a> <span class="note">ASDF/FIND-SYSTEM:LOAD-SYSTEM-DEFINITION-ERROR : Error while trying to load definition for system cl-store from pathname /Users/karstenpoeck/lisp/fork-cl-test-grid/work-dir/agent/quicklisp/dists/quicklisp/software/cl-store-20200925-git/cl-store.asd: This is an unsupported lisp implementation.
Currently only MCL, OpenMCL, Lispworks, CMUCL, SBCL,
CLISP, ECL and AllegroCL are supported.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=1e5oxi2qg7">zbucium</a> <span class="note">CLEAVIR-CST-TO-AST:EVAL-ERROR : ERROR while evaluating compiler-time side effect:
  Filesystem error with pathname #P&quot;/Users/karstenpoeck/.config/.lastfmrc&quot;.
  Either
   1) the file does not exist, or
   2) we are not allowed to access the file, or
   3) the pathname points to a broken symbolic link.</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=154w7zuxam">zenekindarl-test</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT-ACCESSORS| is unbound.</span></td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=17k5u40nlj">zenekindarl</a> <span class="note">COMMON-LISP:UNBOUND-VARIABLE : The variable |@EXPORT-ACCESSORS| is unbound.</span></td><td>0</td><td>1</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td><a href="http://cl-test-grid.appspot.com/blob?key=181lsqa49n">zippy</a> <span class="note">CORE:SIMPLE-PROGRAM-ERROR : Could not munmap memory</span></td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr>
        </tbody>
    </table>
</body>
</html>

