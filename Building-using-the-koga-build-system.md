This page documents the steps needed to build using the new build system which uses a Lisp based metabuilder called koga that outputs [Ninja](https://ninja-build.org/) build files.

# Requirements

The build requirements of clasp must be installed before beginning the build. For each OS listed below install the packages as listed.

* Arch - `pacman -S binutils boost clang gc gmp libbsd libffi libunwind llvm ncurses ninja sbcl`
* Debian/Ubuntu - `apt install -y binutils-gold clang-13 libboost-dev libbsd-dev libclang-cpp13-dev libelf-dev libgc-dev libgmp-dev libncurses-dev libunwind-dev llvm-13 ninja-build sbcl zlib1g-dev`
* Fedora - `dnf install boost-devel clang elfutils-libelf-devel gc-devel gmp-devel libbsd-devel libffi-devel libunwind-devel llvm-devel ncurses-devel ninja-build sbcl zlib-devel`
* MacOS - `brew install bdw-gc boost gmp libffi libunwind-headers llvm ninja pkg-config sbcl`

# Building

Start with a clean Clasp clone on the `ninja` branch. If you have run the waf based build in your clone before then run `./waf distclean` and remove the `build` directory. Also remove any extension clones from the extensions directory and the scraper dependencies located in `/src/scraper/dependencies/`. Koga does not currently support symbolic links in the extensions directory or clones based on `git:` protocol. Then execute the following steps

1. Configure the system and create the build files with `./koga`
2. Build the system with `ninja -C build`
3. Install the system with `sudo ninja -C build install`

# Variants

The default build target is `cclasp-boehmprecise`. This builds iclasp, then aclasp, then bclasp, then cclasp using the Boehm garbage collector in precise mode. The suffix after the dash is a called a variant. The current available variants are:

- boehm - Boehm garbage collector
- boehmprecise - Boehm garbage collector in precise mode
- boehm-d - Boehm garbage collector with debugging symbols
- boehmprecise-d - Boehm garbage collector in precise mode with debugging symbols
- preciseprep - MPS garbage collector. This is only used to analyze Clasp in preparation for the static analyzer.
- preciseprep-d - MPS garbage collector with debugging symbols. This is only used to analyze Clasp in preparation for the static analyzer.

# Targets

There are many intermediate and additional targets available in the Ninja build files. The following is a list of some of the significant ones.

- install: Install the default target. If Jupyter was enabled by koga then this will install Jupyter system kernels also.
- test-[variant]: Run the Clasp regression tests on the specified variant.
- jupyter-[variant]: Install Jupyter user kernels for the specified variant. The clasp binaries used will be the ones in the build directory. This target is primarily used for using JupyterLab in a development repository.
- analyze-[boehm|boehm-d]: Run the static analyzer on the Boehm collector.

# Extensions

The [seqan-clasp](https://github.com/clasp-developers/seqan-clasp/) and [cando](https://github.com/cando-developers/cando/) extensions are compatible with koga. To enable these extensions create a file `config.sexp` in the root of the clasp directory with the following contents then execute the build instructions listed in the previous section.

```lisp
(:extensions (:cando :seqan-clasp))
```

# Configuration

If the configure script does succeed in configuring the build or if you want to adjust the settings you use a plist in `config.sexp`
with the following values. These options can also be passed directly to koga via command line options. For example executing `./koga --debug-lexical-depth` is equivalent to adding `:debug-lexical-depth t` to the plist in `config.sexp`. Extensions can be enabled by passing the names separated with commas, i.e. `./koga --extensions cando,seqan-clasp`

* `:no-sync` — A list of repository names to avoid syncing. This is useful if you are doing development on an extension such as Cando.
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
* `:jupyter` — Enable installation of Jupyter kernels. [default nil]
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
