There is a new dependency for Clasp, so you need to grab this first:
```
sudo apt-get install sbcl
```

Then pull and build the latest Boehm version of clasp using the mps-dev branch (this will take about 3 hours):

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