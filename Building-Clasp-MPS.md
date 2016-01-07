To reproduce the bug in Clasp do the following:

First build the latest version of clasp using the mps-dev branch:

```
git pull origin mps-dev
git checkout mps-dev
```

Build clasp the regular way using:

```
clasp$  make clean; make
```

To build the release and debug versions of MPS clasp use:

```
clasp$ make mps-build
```

Then to lower the amount of memory available to MPS use:

```
export CLASP_MPS_CONFIG="32 32 16 80 32 80"
```

And then to start the release version clasp and try to link a minimal Common Lisp environment:

```
clasp_mps_o -I -f ecl-min
(link-min)
```

It should crash

To start the debug version of clasp - I have not been able to make it crash:

```
clasp_mps_d -f ecl-min
(link-min)
```
