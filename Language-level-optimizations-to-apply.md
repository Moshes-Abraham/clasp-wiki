1) Elide out BLOCK/CATCH/TAGBODY when there is no RETURN-FROM/THROW/TAGBODY.   Every DEFUN creates an implicit BLOCK and if there is no RETURN-FROM then you don't need the overhead of BLOCK.

