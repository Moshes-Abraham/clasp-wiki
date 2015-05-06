1) When defining classes that are exposed to Common Lisp and managed by the garbage collector, multiple inheritance on the C++ side will not work with the compacting MPS garbage collector (Note: Figure out if this is absolutely true).  However, currently we have some examples of this (of multiple inheritance on the C++ side despite it not being allowed) because it is the only way I could figure out to subclass C++ classes in Common Lisp.  It works with the Boehm garbage collector and we need that to build the MPS interface.

For example:
class AstVisitor_O : public core::T_O, public clang::RecursiveASTVisitor<AstVisitor_O> {

AstVisitor_O inherits from T_O and clang::RecursiveASTVisitor<AstVisitor_O> on the C++ side.

However, clasp can only be told about one class that AstVisitor_O inherits from and that has to be core::T_O.
The "registerClasses.py" scraper needs core::T_O to be the FIRST class listed in the base class list as shown above.