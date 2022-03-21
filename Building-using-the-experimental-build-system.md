This page documents the steps needed to build using the experimental build system being developed which uses a Lisp based configuration script that outputs [Ninja](https://ninja-build.org/) build files. This build system is not ready for general use. If you are trying build clasp or cando for general usage then use the waf based builder.

# Requirements

The build requirements of clasp must be installed before beginning the build. For each OS listed below install the packages as listed.

* Arch - `pacman -S binutils boost clang gc gmp libbsd libffi libunwind llvm ncurses ninja sbcl`
* Debian/Ubuntu - `apt install -y binutils-gold clang-13 libboost-dev libbsd-dev libclang-cpp13-dev libelf-dev libgc-dev libgmp-dev libncurses-dev libunwind-dev llvm-13 ninja-build sbcl zlib1g-dev`
* Fedora - `dnf install boost-devel clang elfutils-libelf-devel gc-devel gmp-devel libbsd-devel libffi-devel libunwind-devel llvm-devel ncurses-devel ninja-build sbcl zlib-devel`
* MacOS - `brew install bdw-gc boost gmp libffi libunwind-headers llvm ninja pkg-config sbcl`

# Building

Start with a clean Clasp clone on the `ninja` branch. If you have run the waf based build in your clone before then run `./waf distclean` and remove the `build` directory. Also remove any extension clones from the extensions directory and the scraper dependencies located in `/src/scraper/dependencies/`. Then execute the following steps

1. Configure the system with `sbcl --script configure.lisp`
2. Build the system with `ninja -C build`

This build system does not install Clasp yet. If the build is successful then there will be a Clasp executable named `build/boehm/iclasp-boehm`.

# Variants

The default build target is `cclasp-boehm`. This builds iclasp, then aclasp, then bclasp, then cclasp using the Boehm garbage collector. If you wanted to stop after the aclasp step you would do `ninja -C build aclasp-boehm`. There are many available targets, but the following are the only ones known to work.

* Boehm gc - `iclasp-boehm`, `aclasp-boehm`, `bclasp-boehm`, `cclasp-boehm`, `cclasp-boehm-tests`
* Boehm gc with debugging - `iclasp-boehm-d`, `aclasp-boehm-d`, `bclasp-boehm-d`, `cclasp-boehm-d`, `cclasp-boehm-d-tests`
* Boehm precise gc - `iclasp-boehmprecise`, `aclasp-boehmprecise`, `bclasp-boehmprecise`, `cclasp-boehmprecise`, `cclasp-boehmprecise-tests`
* Boehm precisegc with debugging - `iclasp-boehmprecise-d`, `aclasp-boehmprecise-d`, `bclasp-boehmprecise-d`, `cclasp-boehmprecise-d`, `cclasp-boehmprecise-d-tests`

# Extensions

The only extensions that are currently compatible with this build system are [seqan-clasp](https://github.com/clasp-developers/seqan-clasp/) and [cando](https://github.com/cando-developers/cando/). To enable these extensions create a file `config.sexp` in the root of the clasp directory with the following contents then execute the build instructions listed in the previous section.

```lisp
(:extensions (:cando :seqan-clasp))
```

Cando currently only builds using the Boehm precise variant. To build this variant execute the following.

```
ninja -C build cclasp-boehmprecise
```

# Configuration

If the configure script does succeed in configuring the build or if you want to adjust the settings you use a plist in `config.sexp`
with the following values.


* `:build-mode` — Define how clasp is built. [default :faso]
  - `:bitcode` compiles to bitcode and thinLTO is used to link everything.
    This gives the fastest product but linking takes a long time.
  - `:object` produces object files and regular linking is used.
    This is probably not as fast as bitcode (maybe a few percent slower)
    but it links fast.
  - `:faso` generates faso files. This is good for development.
  - `:fasobc` generates fasobc files.
  - `:fasoll` generates fasoll files.
  - `:fasl` generates fasl files.
* `:build-path` — The path for build files such as the Ninja build file. 
  [default #P"build/"]
* `:parallel-build` — Build clasp in parallel. [default t]
* `:prefix` — Where Clasp is install. [default "/usr/"]
* `:extensions` — A list of extensions. [default nil]
* `:cst` — [default t]
* `:clang-cpp` — If t use clang-cpp otherwise use the individual clang 
  libraries. [default t]
* `:compile-file-parallel` — [default t]
* `:force-startup-external-linkage` — Use external-linkage for startup 
  functions. [default t]
* `:unwinder` — [default :gcc]
* `:jobs` — The number of jobs during build. If not specified then a value will
  be picked based on the number of CPU cores. [default nil]
* `:always-inline-mps-allocations)` —
* `:address-sanitizer` — [default nil]
* `:memory-sanitizer` — [default nil]
* `:thread-sanitizer` — [default nil]
* `:debug-dtree-interpreter` — Generate dtree interpreter log [default nil]
* `:debug-dtrace-lock-probe` — Add a Dtrace probe for mutex lock acquisition
  [default nil]
* `:debug-stackmaps` — print messages about stackmap registration [default nil]
* `:debug-assert` — Turn on DEBUG_ASSERT [default t]
* `:debug-assert-type-cast` — Turn on type checking when passing arguments
  [default nil]
* `:source-debug` — Allow LOG messages to print - works with CLASP_DEBUG 
  environment variable [default nil]
* `:debug-jit-log-symbols` — Generate a log of JITted symbols in 
  `/tmp/clasp-symbols-<pid>` [default nil]
* `:debug-guard` — Add guards around allocated objects [default nil]
* `:debug-guard-validate` — Add quick checking of guards [default nil]
* `:debug-guard-backtrace` — Add allocation backtraces to guards [default nil]
* `:debug-guard-exhaustive-validate` — Add exhaustive, slow, checks of guards
  [default nil]
* `:debug-trace-interpreted-closures` — [default nil]
* `:debug-environments` — [default nil]
* `:debug-release` — Turn off optimization for a few C++ functions; undef this 
  to optimize everything [default nil]
* `:debug-cache` — Debug the dispatch caches - see cache.cc [default nil]
* `:debug-bitunit-container` — Prints debug info for bitunit containers 
  [default nil]
* `:debug-lexical-depth` — Generate tests for lexical closure depths 
  [default nil]
* `:debug-flow-tracker` — Record small backtraces to track flow [default nil]
* `:debug-dynamic-binding-stack` — dynamic variable binding debugging
  [default nil] 
* `:debug-values` — turn on printing `(values x y z)` values when 
  `core:*debug-values*` is not nil [default nil]
* `:debug-ihs` — [default nil]
* `:debug-track-unwinds` — Count cc_unwind calls and report in TIME 
  [default nil]
* `:debug-no-unwind` — Debug intrinsics that say they don't unwind but actually 
  do. [default nil]
* `:debug-startup` — Generate per-thread logs in `/tmp/dispatch-history/**` of 
  the slow path of fastgf [default nil]
* `:debug-rehash-count` — Keep track of the number of times each hash table has 
  been rehashed [default nil]
* `:debug-monitor` — generate logging messages to a file in /tmp for non-hot 
  code [default nil]
* `:debug-monitor-support` — Must be enabled with other options - do this 
  automatically? [default nil]
* `:debug-memory-profile` — Profile memory allocations total size and counter
  [default nil]
* `:debug-bclasp-lisp` — Generate debugging frames for all bclasp code - like 
  declaim [default nil]
* `:debug-cclasp-lisp` — Generate debugging frames for all cclasp code - like 
  declaim [default t]
* `:debug-count-allocations` — count per-thread allocations of instances of 
  classes [default nil]
* `:debug-compiler` — Turn on compiler debugging [default nil]
* `:debug-verify-modules` — Verify LLVM modules before using them [default nil]
* `:debug-long-call-history` — The GF call histories used to blow up - this 
  triggers an error if they get too long [default nil]
* `:debug-bounds-assert` — check bounds [default t]
* `:debug-gfdispatch` — debug call history manipulation [default nil]
* `:debug-fastgf` — generate slow gf dispatch logging and write out dispatch 
  functions to `/tmp/dispatch-history-**` [default nil]
* `:debug-slot-accessors` — GF accessors have extra debugging added to them
  [default nil]
* `:debug-threads` — [default nil]
* `:debug-stores` — insert a call to `cc_validate_tagged_pointer` everytime 
  something is written to memory [default nil]
* `:debug-ensure-valid-object` — Defines `ENSURE_VALID_OBJECT(x)->x` macro - 
  sprinkle these around to run checks on objects [default nil]
* `:debug-quick-validate` — quick/cheap validate if on and comprehensive 
  validate if not [default nil]
* `:debug-mps-size` — check that the size of the MPS object will be calculated 
  properly by obj_skip [default nil]
* `:debug-mps-underscanning` — Very expensive - does a 
  `mps_arena_collect`/`mps_arena_release` for each allocation [default nil]
* `:debug-dont-optimize-bclasp` — Optimize bclasp by editing llvm-ir 
  [default nil]
* `:debug-recursive-allocations` — Catch allocations within allocations - MPS 
  hates these [default nil]
* `:debug-alloc-alignment` —
[default nil]
catch misaligned allocations
* `:debug-llvm-optimization-level-0` — [default nil]
* `:debug-slow` — Code runs slower due to checks - undefine to remove checks
  [default nil]
* `:human-readable-bitcode` — [default nil]
* `:debug-compile-file-output-info` — [default nil]
* `:config-var-cool` — mps setting [default t]
* `:ar` — Pathname of ar binary. [default nil]
* `:cc` — Pathname of cc binary. [default nil]
* `:cxx` — Pathname of cxx binary. [default nil]
* `:git` — Pathname of git binary. [default nil]
* `:llvm-config` — Pathname of llvm-config binary. [default nil]
* `:nm` — Pathname of nm binary. [default nil]
* `:pkg-config` — Pathname of pkg-config binary. [default nil]
