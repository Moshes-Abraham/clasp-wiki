# Building only the clasp_mps_d and clasp_mps_o executables.

You can skip compiling all of the clasp Common Lisp source code for now.

Get the latest version of the mps-dev branch and then build the executables.

```
clasp$ make mps-build
```

To build just the debug or the release versions use:
```
clasp$ cd src/main
main$ make mps-debug-cxx
main$ make mps-release-cxx
```

To run tests that should crash and reveal problems you can use...
```
clasp_mps_d -I -f ecl-min
(clean-system :init :no-prompt t)
(compile-min)
(link-min)
```

# Instructions for building the MPS version of Clasp once it is working fully

Pull and build the latest Boehm version of clasp using the mps-dev branch (this will take about 3 hours):

```
clasp$ git pull origin mps-dev
clasp$ git checkout mps-dev
clasp$ make clean; make
```

To build the release and debug versions of MPS clasp (about 20 min) use:

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

#More tests of Clasp 

You can do the following with both clasp_boehm_o and clasp_mps_o and observe how clasp_mps_o may crash when clasp_boehm_o does not.

```
clasp_boehm_o -I -f ecl-min
(clean-system :init :no-prompt t) ; clear out compiled bitcode files
(compile-min)                     ; Compile a minimal Common Lisp system
```

Try the same thing with ```clasp_mps_o -I -f ecl-min```.  