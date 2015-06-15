(done) consp, car, cdr, rplaca, rplacd
atom
null
endp
listp
symbolp
+other predicates
<stassats> a useful transformation: (char-equal x #\a) => (or (char= x #\A) (char= x #\a))