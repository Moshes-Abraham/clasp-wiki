# Introduction

Clasp is an implementation of Common Lisp primarily designed for compatibility with C++-language programs and libraries.

Note that Clasp is a work in progress, as is this manual.

## Conformance

Clasp conforms with the requirements of ANSI INCITS 226-1994 (R2004) with some exceptions, listed below in the "Lisp" section. Any deviation from the standard not listed there is a bug, and should be reported (see "Contributing").

## Distribution

At present, the developers do not make Clasp binaries available. Clasp is open source, and available on-line at https://github.com/clasp-developers/clasp.

## Building

TODO

## Contributing

The developers welcome bug reports and patches. Both should ideally be mediated through the GitHub interface at https://github.com/clasp-developers/clasp.

Discussions of Clasp development are mostly carried out on Freenode's #clasp channel.

## Credits

Clasp is the project of Dr. Christian Schafmeister. Additional contributions have been made by Alex Wood, Karsten Poeck, and many other contributors as seen in the Git history.

Clasp's source code is derived substantially from that of Embeddable Common Lisp. Code from SBCL and SICL has been incorporated as well. Most notably, the compiler is SICL's Cleavir compiler with some minor customizations.

# Starting and Stopping

The Clasp executable accepts many different command line arguments. You can get the most up to date summary by passing `--help`. Here are some important ones:

- `--noinform`: Skip messages at startup.
- `--noprint`: Start a read-eval loop instead of a read-eval-print loop, and don't prompt. This is intended for scripts (e.g. piping a list of forms to Clasp).
- `--disable-debugger`: Set things up so that if the default debugger would be entered, Clasp quits with a backtrace and nonzero exit status instead. `*debugger-hook*` and `ext:*invoke-debugger-hook*` (below) work as usual, i.e. this setting does not affect them.
- `--non-interactive`: Rather than starting a REPL, quit. This is intended to be used with `--eval` and `--load`. Implies `--disable-debugger`.
- `--feature feature`: Intern "feature" as a keyword and push it to `*features*`.
- `--eval form`: Evaluate the given form. `--eval` and `--load` options are processed in order from left to right.
- `--load filename`: `cl:load` the given file. Intended for convenience, since `--eval (load ...)` could involve annoying quotation issues.
- `--norc`: Do not load `~/.clasprc` (see below).

If the file `~/.clasprc` exists, Clasp will `cl:load` it before processing `--eval` and `--load` options and starting the REPL.

To exit Clasp, the `ext:quit` function can be used. If provided an integer argument, it's used as the exit status; the default is zero.

# Lisp

As mentioned, Clasp is an implementation of ANSI Common Lisp. The following subsections detail intentional deviations from the standard, some extensions to standard functionality, and notes on optimizing Lisp programs to run well within Clasp. (Extensions not closely related to standard systems are explained in their own sections below.)

## Evaluation and Compilation

Clasp expands compiler macros essentially unconditionally. That is, provided the operator is not declared `notinline`, the compiler will attempt to expand compiler macros. If compiler macroexpansion signals, this signal will be recorded and reported by the compiler. If compiler macroexpansion errors out, the compiler will abandon expansion and use the unexpanded form, while noting the error for display.

`ext:with-current-source-form` is a useful macro to allow error messages from macroexpanders and compiler-macro-expanders to have more specific source information. See its docstring for more information.

[We have a symbol macro function accessor, but I don't think it will work for non-global symbol macros, so it can't exactly be documented]

## Types and Classes

`typep` calls can be efficiently compiled only if the second argument, the type specifier, is constant. Clasp's compiler will process the type specifier and generate code to check for objects of that type directly, avoiding the usual runtime cost of interpreting the type.

Types defined by `deftype` use a "type expander" function analogous to a macro expander function. A type expander is a function of two arguments, a type specifier and an environment. When called on an appropriate specifier and environment, it computes and returns another type specifier. Type expanders are accessible through the `ext:type-expander` accessor.

### Disjointness

Unless otherwise specified, types Clasp defines as extensions can be considered to be in a disjointness relationship with other types, as in CLHS 4.2.2 "Type Relationships". That is, if Clasp defines a type `foo`, you can assume that `foo` is not a subtype of `hash-table`, or `cons`, or so on, and vice versa, unless it is explicitly stated to be. But just as in 4.2.2, Clasp extension types may be subtypes of `structure-object` or `standard-object` without this being explicitly noted here.

## Data and Control Flow

[specialp and symbol-constantp aren't really regular enough to document]

[core:out-of-extent-unwind should perhaps be moved to ext]

`defsetf`, `define-setf-expander` etc. define a "setf expander" function analogous to a macro expander function. A setf expander is a function of two arguments, a place and an environment. When called an appropriate place and environment, the expander computes and returns the values used by `setf`. Setf expanders are accessible through the `ext:setf-expander` accessor.

## Iteration

`loop` supports iteration over general sequences (see below) through a for-as-sequence subclause. This is identical to the subclause in SBCL. The syntax is `being {each | the} {element | elements} {of | in}`. For example, `(loop for x being each element in '(1 2 3) do (print x))`.

## Objects

CLOS, as part of Common Lisp, is fully supported.

### Metaobject Protocol

The Metaobject Protocol, as described in AMOP [reference], is supported. Undocumented deviations from AMOP are bugs and should be reported, as with the CL standard.

Symbols relating to MOP are exported from the "CLOS" package.

### Generic function dispatch efficiency

Clasp uses a new system for generic function dispatch designed by Dr. Robert Strandh. [Paper reference goes here.] Essentially, after a few calls to a generic function, a just-in-time compiler will install a discriminating function for it that can pass control to the correct effective method very efficiently. This means that calls with arguments that all have the same specializers as those of a previous call will in general be more efficient.

For some applications, the specializers a function will be called with are known beforehand, and the runtime overhead of the just-in-time compilation would be unfortunate. Clasp defines an interface to take care of most of the compilation early: The `clos:satiate` function. See it's docstring for more info.

This system is still under development and will be improved further.

### Miscellany

A consequence of the dispatch method described above is that obsolete instances are updated as soon as they are used as an argument to any generic function call - not just to slot accessors. This is allowed by the standard, but may surprise some programmers.

## Structures

## Conditions

In addition to `cl:restart-name`, Clasp provides some readers to introspect about restarts, for advanced users (e.g. writing your own debugger): `ext:restart-function` returns the function called by `cl:invoke-restart`, and `ext:report-function`, `ext:interactive-function`, and `ext:interactive-function` return the corresponding arguments in `cl:restart-bind`. These will always be appropriate functions, so for example `ext:report-function` will always return a function of one stream argument, but if no `:report-function` was provided it will report the restart in Clasp's default way. The identities of these returned functions cannot be relied on, i.e. they may not be identical to those provided to `cl:restart-bind`.

There is also `ext:restart-associated-conditions`, which returns a list of conditions associated (by `cl:with-condition-restarts`) with the restart in the current dynamic environment.

## Symbols

## Packages

Clasp supports package-local nicknames, through an interface based on that of SBCL's. A package-local nickname is a nickname for a package that is only active when some other package is in place. For example, if the package "FOO" has "B" as a package-local nickname for package "BAR", then while `*package*` is the `foo` package, the prefix "B:" will be read as if it was "BAR:".

Local nicknames may be specified in `defpackage` through the `(:local-nicknames (nickname package-name)*)` extended options. `nickname` must be a string designator and `package-name` a package designator - both are unevaluated. The functions `ext:package-local-nicknames`, `ext:add-package-local-nickname`, `ext:remove-package-local-nickname`, and `ext:package-locally-nicknamed-by-list` can be used for a more programmatic interface.

## Numbers

There are two types of floats, `single-float` and `double-float`. `short-float` is synonymous with the former and `long-float` is synonymous with the latter, per the standard's requirements. `single-float` is in the IEEE754 binary32 (single) format, and `double-float` in binary64 (double) format. The representation of a float as bits can be interconverted with a float using the functions `ext:single-float-to-bits`, `bits-to-single-float`, `double-float-to-bits`, and `bits-to-double-float`. These functions take or return nonnegative integers; for example `(logbitp 31 (ext:single-floats-to-bit float))` returns whether the sign bit is set.

## Characters

Clasp supports Unicode by default. `code-char` and `char-code` work with Unicode codepoints. Unicode character names are also supported, e.g. `(princ #\GREEK_SMALL_LETTER_LAMDA) -> λ`. `(defun λ(n)(* 2 n)) (λ 32) -> 62`is also possible.

Type `character` includes all characters in Unicode. Type `base-char` includes only single byte characters, i.e. Basic Latin and Latin-1 Supplement.

## Conses

## Arrays

In Clasp, arrays with no fill-pointer, displacement, or express adjustability are simple (as in `simple-array`), and arrays that have any of these are not. Additionally, Clasp implements multidimensional arrays - even ones that are simple in this sense - as if they were displaced to an underlying one dimensional array. As such, it is most efficient to work with one-dimensional simple arrays directly.

## Strings

## Sequences

### Extensible Sequences

[The extensible sequences protocol described by Chris Rhodes](http://www.doc.gold.ac.uk/~mas01cr/papers/ilc2007/sequences-20070301.pdf) [FIXME: Real citation] is supported. Symbols related to the protocol are external in Clasp's "SEQUENCE" package. This protocol allows programmers to define their own sequence classes that work efficiently with standard Common Lisp functions. It is recommended that programmers consult other resources, such as Dr. Rhodes' paper, for more information on how to use this protocol effectively.

To summarize: Programmers wishing to make a custom sequence class must ensure their class has `cl:sequence` as a superclass. (Note that `sequence` is itself abstract, so if a custom class needs to have e.g. slots, it should also be a subclass of `standard-object` or something like it.) Methods on `elt`, `(setf elt)`, `length` applicable to objects of the class must be defined for any sequence functions to work; an applicable method on `make-sequence-like` must be defined for creation of this sequence to work; and an applicable method on `adjust-sequence` must be defined for destructive operations to work. Standard sequence functions will then operate correctly with these sequences, as will `make-sequence` and `coerce`.

For efficiency, programmers may also define applicable methods on `make-sequence-iterator`, or less efficiently but more simply, on `make-simple-sequence-iterator`, `iterator-step`, `iterator-endp`, `iterator-element`, `(setf iterator-element)`, `iterator-index`, and `iterator-copy`.

Note that because the `sequence:` generic function cognates to `cl:` sequence functions are defined to have the same behavior in almost all cases, Clasp takes the view that they need not be called. For example, a call to `cl:find` with a custom sequence object _may_ result in a call to `sequence:find`, but may not. In other words the cognates are considered optional, and only possibly useful for optimization. This is still in flux. If you think it's a bad idea, contact a maintainer to talk.

As a small extension to the extension, if a custom sequence object does not implement enough of the protocol for a sequence function to complete, it will signal an error of type `sequence:protocol-unimplemented`. The reader `sequence:protocol-unimplemented-operation` can be used to get the name of the operation that failed from these conditions.

## Hash Tables

`make-hash-table` supports additional keyword arguments.

`:weakness` can be used to indicate that the garbage collection may collect individual hash table entries even when the hash table itself is live, in certain circumstances. At present, only weak-key hash tables are supported: when the weakness argument is `:key`, the hash table's reference to the key of a table entry is _weak_, and if there are no non-weak references to a key, it is collectable. See the "Garbage Collection" section below for more information on weak references. If the weakness parameter is passed as `nil`, or not passed, the hash table does not contain weak references.

`:thread-safe` can be used to make hash table access safe across multiple threads. If a thread-safe argument is not passed, or `nil` is passed, the hash table cannot safely be written to or read from multiple threads simultaneously (see "Memory Model", below, for a brief explanation of terminology). If the thread-safe argument is true, the implementation will ensure that accesses can be carried out from multiple threads simultaneously safely. This does impose a small performance penalty, which is why it is not the default.

If a `:test` other than a standard equality predicate is passed, `:hash-function` must be specified as well. The hash function should be a designator for a function of one argument that is analogous to `sxhash`, i.e. `(funcall test x y)` implies `(= (funcall hash-function x) (funcall hash-function y))` and so on. This will create a "custom" hash table that can be used with the standard hash table functions like `gethash`, with the exception that at the moment, attempting to dump a custom hash table has undefined consequences.

## Filenames

## Files

## Streams

### Gray streams

The Gray stream interface as described in ANSI committee issue "STREAM-DEFINITION-BY-USER" (readable, e.g., [on Kent Pitman's website](http://www.nhplace.com/kent/CL/Issues/stream-definition-by-user.html)) is supported. Symbols are exported from package "GRAY". We recommend programmers use a multi-implementation compatibility layer such as [trivial-gray-streams](https://common-lisp.net/project/trivial-gray-streams/) rather than use Clasp's implementation directly.

Gray streams allow programmers to define their own stream classes with custom behavior that work with standard Common Lisp functions. It is recommended that programmers consult another resource, such as the trivial-gray-streams documentation, for more information on how to use this interface effectively.

## Printer

When `format`'s control string argument is constant, the compiler will process it early, so that the runtime doesn't have to. This improves runtime speed but increases code size.

## Reader

## System Construction

## Environment

### Stepper

`cl:step` can be used to step through compiled code as partially described in the standard. Currently, the stepper can only stop on forms that happen to be compiled as calls, though this may be improved in the future.

Code is steppable if it is compiled with `debug 3` optimization settings, or is within the `step` macro. While unsteppable code is being executed, the stepper will not stop.

Clasp further defines some aspects of stepping for the sake of editor/debugger integration. When the stepper pauses execution, a condition of type `cl:step` is passed to the debugger. This condition will print with the source form for the call. Similarly to `cl:break`, `*debugger-hook*` is bound to `nil`, but `ext:*invoke-debugger-hook*` (described below) can still be used for interception. The following restarts are available from a `step` condition:

- `cl:continue`: Continue without stepping. The stepper will not invoke the debugger again.
- `clasp-debug:step-into`: Continue stepping. If the function to be called is steppable, the stepper will pause within it, and otherwise stepping will proceed after the call.
- `clasp-debug:step-over`: Continue stepping, but not into the call the stepper is on. Stepping will proceed after the call is exited (either by normal return or a non-local exit).

# C++ Interface

TODO. See [this page](https://clasp-developers.github.io/clbind-doc.html) for now.

# Foreign Function Interface

Clasp can interact with C programs and libraries through its Foreign Function Interface (FFI). Symbols relating to this interface are external in package "CLASP-FFI". However, it is recommended for most applications that you use a cross-implementation wrapper layer, specifically [CFFI](https://common-lisp.net/project/cffi/).

TODO

# REPL

Clasp's built in read-eval-print loop supports various commands in addition to evaluating Lisp forms. These commands consist of lines beginning with a Lisp keyword, followed possibly by additional arguments. The most up to date documentation for this interface is the on-line help system, obtainable with the command `:help`.

Clasp has a built in debugger, which will be entered by `invoke-debugger` by default. `:help` can describe the debugger commands as well. Some basic commands are `:b` to print a backtrace, `:rN` to invoke the Nth restart, `:v` to print local variables in the frame, and `:up`, `:down`, and `:go` for navigating frames.

In addition to the standard `*debugger-hook*`, Clasp has `ext:*invoke-debugger-hook*`. This is a similar hook function, but it will be tried before `*debugger-hook*`, and importantly, will be called even for `break` (which binds `*debugger-hook*` to `nil` per the standard). This can be used to set up your own debugger in an IDE.

In the debugger, the function `ext:tpl-frame` can be used to return a representation of the current frame suitable for the programmatic debug interface described below, and `ext:tpl-argument` and `ext:tpl-arguments` can be used to retrieve arguments.

In some applications, it's useful for the program to exit rather than exit a debugger. The functions `ext:disable-debugger` and `ext:enable-debugger` can be used to set whether the debugger will be entered. These only affect the **built in** debugger, and they do not affect `*debugger-hook*` or `ext:*invoke-debugger-hook*`.

# Debug interface

For advanced users, such as those developing development tools such as debuggers to use with Clasp, a programmatic interface to debug information is provided by the `CLASP-DEBUG` package.

The `with-stack` and `call-with-stack` operators allow `frame` objects, representing part of the current control stack, to be interrogated. These frame objects have several readers: `frame-function`, `frame-arguments`, `frame-locals`, `frame-source-position`, and `frame-language`. More specific information about the function can be obtained with `frame-function-name`, `frame-function-lambda-list`, `frame-function-source-position`, `frame-function-form`, `frame-function-documentation`, and `disassemble-frame`.

Note that frames necessarily have dynamic extent, because the local variables, arguments, and functions they refer to may be dynamic-extent themselves.

To navigate frames smoothly, a notion of "visibility" exists. Frames can be "invisible" if they aren't of interest to users. This includes things like internal system code. Of course, the concept of visiblity can change. Frame visibility is controlled by the `*frame-filters*` variable, which holds a list of function designators: a frame is visible if none of the functions return a true value when given the frame as an argument. As such, all frames are considered visible if `*frame-filters*` is bound to `nil`.

`up` and `down` can be used to navigate visible frames, while `frame-up` and `frame-down` ignore visibility. `map-stack`, `list-stack`, and `map-indexed-stack` can be used to perform manipulations on all frames at once.

`with-truncated-stack` and `with-capped-stack` can be used as hints to `with-stack` (and therefore debuggers) that only a portion of the control stack is of interest. For example, a function that signals an error can use `with-truncated-stack` to ensure that lower debugger frames are not included in backtraces.

`print-backtrace` is provided as a simple way to print a current backtrace, without needing to use `with-stack` or anything.

# Multiprocessing

Multiprocessing is supported. Symbols relating to multiprocessing are exported from the "MP" package.

## Processes

A process is a Lisp object representing a distinct thread of execution. Each process evaluates a call to a Lisp function, and exits when that call would finally return values. Processes have names for debugging purposes. Processes are "nascent" or "not yet started" if they haven't yet begun evaluating, "active" if they have begun evaluating, "suspended" if that evaluation has been paused by `process-suspend`, and "exited" if they have finished evaluation (normally or by aborting).

Processes have type `process`. `make-process` creates a new process but does not start it. `process-start` enables a process, and `process-run-function` both creates and enables a process. The name of a process can be retrieved with `process-name`. `process-active-p` can be used to query whether a process is active. `process-suspend`, `process-resume`, `interrupt-process`, and `process-kill` interfere with a process's evaluation. `process-join` waits until a process until it completes, and then returns the values its function returned, or signals an error of type `process-join-error` if the process ended abnormally. Within a process, `exit-process` can be used to end the process's evaluation immediately, and `abort-process` to do so abnormally; in either case the dynamic environment is properly unwound. `all-processes` gets a list of all enabled processes. The variable `*current-process*` is bound in any process to that process. Consult the docstrings of these functions for more information.

## Special variables

Bindings of special variables (by `let`, `progv`, lambda lists, etc.) are thread-local. That is, executing a binding form for a variable will not affect that variable's value in other threads. The global value - from `symbol-value` - is, in contrast, shared between threads.

## Mutexes

A mutex (short for "MUTual EXclusion"), or lock, can be used to control access to a shared resource by multiple processes.

Mutexes have type `mutex`. A mutex is created with `make-lock`, or `make-recursive-mutex` for a recursive mutex. `get-lock` and `giveup-lock` obtain and release exclusion on a mutex, respectively. `mutex-name` retrieves any name of a mutex given at creation.

## Shared Mutexes

TODO

## Condition Variables

TODO

## Memory Model

Clasp does not have a formal memory model. Here is a sketch of one: Two accesses of a place are `concurrent` if they take place in different threads and are not excluded from running simultaneously by locks. Two concurrent accesses `conflict` if at least one is a write. If a conflicting access is not _atomic_ the program has undefined behavior (e.g. tearing).

Some accesses are atomic but _unordered_, meaning that there is not necessarily a modification order to the place that is observed by all threads, e.g. one thread may see writes occur in a different order from another thread. Some accesses are _sequentially consistent_, meaning that there is such a globally observable modification order, and furthermore that all sequentially consistent accesses have a globally observable order.

Places may be complex, indeed completely custom. Clasp defines atomicity of some simple places; other places, and more complex modification operations, should hopefully be understandable from those. For example, to setf the `second` of a list, one `cdr` must be read before a `car` is written, and each of these individual accesses is atomic while the overall access is not.

In general Clasp tries to guarantee unordered atomicity, but does not always succeed, and in some cases it's probably not possible.

Note that in this context "atomic" does not necessarily mean "lock-free".

Places that can be accessed unorderedly are: `car`, `cdr`, `symbol-value`, `symbol-plist`, `symbol-function`/`fdefinition`, `compiler-macro-function`, `ext:setf-expander`, `ext:type-expander`. Access to the elements of simple one-dimensional arrays should be unordered, except for integer element types smaller than `(unsigned-byte 8)`. Access to `standard-object` and `structure-object` slots (of `:instance` or `:class` allocation) should also be unordered.

## Atomics

Access can be guaranteed atomic by using the `atomic` macro. That is, `(atomic place)` is a place that can be accessed atomically, or else an error will be signaled. Clasp defines `car`, `cdr`, `first`, `rest`, `symbol-value`, special variables, `symbol-plist`, `standard-instance-access`, `slot-value`, `clos:slot-value-using-class`, and `svref` as atomically accessible, as well as `the` place or macro places that expand to these places. Additional atomically accessible places can be defined with the `define-atomic-expansion` macro. See its documentation string for more information. Additionally, documentation on atomic access may be available with kind `atomic`; e.g. try `(documentation 'symbol-value 'mp:atomic)`.

## Compare-and-swap

The `mp:cas` macro can be used to execute an atomic compare-and-swap of atomically accessible places. See its docstring for more information. `cas` is used to define higher order atomic read-modify-write operations provided by Clasp: `atomic-update`, `atomic-incf`, `atomic-decf`, `atomic-push`, `atomic-pop`, and `atomic-pushnew`. The first is a general operator analogous to what `define-modify-macro` operators do, while the others are analogous to their standard versions. `-explicit` variants can be used to explicitly specify the order of the operation.

## Fences

The `mp:fence` macro can be used to establish memory fences of a specified order.

# Introspection

Information about objects is stored and accessible. This is primarily intended for editor integration, but the functions can be used in any context. It is not recommended that they be used for purposes other than human understanding, however - it can sometimes be dropped or inaccurate. These mechanisms are similar to the standard `documentation` function.

`ext:function-lambda-list` can be used to get the lambda list of a function object, and `ext:compiled-function-name` its name.

`ext:source-location` returns a list of source locations for a symbol or object. Source locations are of type `ext:source-location`; they contain a pathname accessible with `ext:source-location-pathname`, and a file offset (as from `file-position`) accessible with `ext:source-location-offset`.

# Sockets

A low level networking API based on SBCL's (which is in turn based on BSD sockets) is available in package "SB-BSD-SOCKETS".

TODO

# Serve Event

TODO

# Garbage Collection

Symbols related to garbage collection are exported from the "GCTOOLS" package.

The function `garbage-collect` forces a garbage collection.

`finalize` registers a finalizer function for an object. When the object is collected, the function will be called with no arguments. Note that this function should not close over the object, because then the closure will keep that object alive indefinitely.

# POSIX
## Signal Handling
Handlers for standard POSIX signals can be defined in Clasp using the `ext:enable-interrupt` function, which excepts a keyword to identify the type of signal (e.g. `:sigpipe` for `SIGPIPE`). If a Lisp function is used as the handler, it must be a function of one argument, the signal number. `ext:enable-interrupt`, or `ext:ignore-interrupt` and `ext:default-interrupt`, can be used to set the handler to the ignore-signal handler or the default handler respectively, analogous to `SIG_IGN` and `SIG_DFL`. The current handler function, if there is one, can be retrieved with `ext:get-signal-handler`.
## Further posix interfaces
`ext:stat` and `ext:fstat` wrap the corresponding posix-interfaces. Use `ext:file-stream-file-descriptor` to get the file-descriptor for a stream.
The environment can be accessed with `EXT:SETENV`and `EXT:GETENV`
Working directories can be accessed with `EXT:GETCWD`and `EXT:CHDIR`.  

# Interfaces outside of POSIX
## File System
`ext:rmdir` to delete a directory, `EXT:RMTREE` allows to remove a whole directory tree
## Other interfaces
`ext:quit` to leave clasp