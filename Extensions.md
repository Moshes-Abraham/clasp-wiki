Package-local nicknames
-----------------------

If a string is a "local nickname" for some package A within some other package B, then when `*package*` is B, `find-package` (and all implicit uses thereof, e.g. in `read`) will return A given the string.

Local nicknames are usually specified in `defpackage`, with the `:local-nicknames` option. Like so:

```common-lisp
(defpackage foo (:use #:cl) (:local-nicknames (#:e #:ext)))

(in-package #:foo)

(e:package-local-nicknames *package*)
; => (("E" . #<PACKAGE EXT>))
```

"E" in the package prefix means EXT, as long as `*package*` is the FOO package.

Interface cribbed from SBCL: The `:local-nicknames` option, and `package-local-nicknames`, `add-package-local-nickname`, `remove-package-local-nickname`, `package-locally-nicknamed-by-list`. See docstrings.

Extensible sequences
--------------------

Clasp supports [the SEQUENCE extension as described by Dr Christophe Rhodes](http://research.gold.ac.uk/2344/1/sequences-20070301.pdf), which allows standard functions like `count` to work on user-defined classes, provided they implement a small protocol. The relevant functions are accessible from the SEQUENCE package.

Clasp adds a few helper functions and macros, and as a small deviation from the system as described, does not guarantee that custom methods on `sequence:find` etc. are called in all situations. It does guarantee that the standard functions and built-in methods will work on general sequences, to be clear, but sometimes optimization opportunities rule out calling the generic function. See src/clos/sequences.lsp for more details.