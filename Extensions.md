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