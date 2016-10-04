# Linux
Adapt paths as necessary. Required prerequisites are: a sane compiler environment for C and C++, boehm, cmake, boost of recent enough versions. Debian stable unfortunately does not yet sport high enough versions of the latter two.

1. `git clone https://github.com/drmeister/externals-clasp ~/externals-clasp`
2. `git clone https://github.com/drmeister/clasp ~/clasp`
3. `cd ~/externals-clasp && make`
4. `cd ~/clasp && echo "EXTERNALS_CLASP_DIR = $HOME/externals-clasp" > local.config`
5. `make`

# OS X
TBD