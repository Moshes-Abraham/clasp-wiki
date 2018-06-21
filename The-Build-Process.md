# Bootstrap Stages

See also [docs/bootstrap.rst](https://github.com/clasp-developers/clasp/blob/dev/docs/bootstrap.rst) until the two get merged.

## `iclasp`
is an interpreter for a subset of CL written in C++.

iclasp is already capable of calling the LLVM functions (see the `llvm-sys` package).

iclasp expands macros repeatedly, every time they are reached. This makes it rather slow with `loop` and friends.

## `aclasp`
is iclasp after loading a minimal CL system that is capable of `compile-file`-ing a subset of CL. aclasp is written in  this subset of CL, i.e. aclasp is just smart enough to self-compile. `compile-file` happens by calling the LLVM machinery at runtime.

`./waf build_rboehm` starts iclasp and has it load the aclasp Common Lisp source code as interpreted code; i.e. absolutely no Common Lisp compilation happens up to this point.

At this point aclasp is used to compile itself (i.e. calling `compile-file` on the CL source files that are implementing aclasp). When a file is successfully compiled, it is loaded into the running image, which leads to a gradual speedup of this process of compilation.

`./waf build_aboehm` then links the `compile-file`'d code into a fasl called `aclasp-boehm-image.fasl`. Run `iclasp-boehm` with this image and you get what you get when you run `./waf build_rboehm`, but everything is compiled now (i.e. faster).

## `bclasp`
is aclasp compiling and loading a few more files that turn aclasp into a complete CL system that is now able to run [Cleavir](http://metamodular.com/cleavir.pdf), which is a modern full-blown CL compiler that requires full CL support to run, CLOS included.

## `cclasp`
is the self-compilation of/with Cleavir, i.e. it's created by loading Cleavir into `bclasp` and recompiling everything.

# Plans for a bootstrap refactor

## Current issues and rationale for a refactor
* The same codebase is used to build all the different stages of the bootstrap. Because of this the code has many `#+(or bclasp cclasp)` like reader conditionals, and parts of the codebase is written with compromises that are needed to be made only to able to execute it an early (dumb) stage of the bootstrap.
* Changing the runtime (e.g. memory layout, GC kind/operation, supported object types, etc) must be done so that it works throughout all the stages of the bootstrap, even though they are often unnecessary complexity for the earlier stages that are only used as an intermediate jumping stone to bring the later stages to life.
* The codebase is harder to understand/approach because of the lost clarity and the sheer size that is there even in the early stages.
* When the stages are properly isolated, i.e. stage-n only uses a well defined artifact of stage-n-1, and only to produce link artifacts for stage-n, then rebuilding earlier stages should be needed much less frequently, and opens up more freedom to change the runtime in later stages.
* The build scripts for independent stages will become much simpler; i.e. all of the `stage_char` related stuff can be eliminated.

## Requirements (plus the optional ones)

* Be able to bootstrap from multiple "ground floor", i.e. clang (currently) and CL (hypothetical for now)

## Proposed design

* Create a git branch for each stage from the current `dev`:
  * stage-1 - what's currently called iclasp
  * stage-2 - aclasp
  * stage-3 - bclasp
  * stage-4 - cclasp
  * stage-5+ - as needed when we need to introduce a new feature that we want to use/rely on in Cleavir, or other parts of the runtime or compiler implementation.
* `dev` or `master` will always hold the currently latest stage
* A `bootstrap.sh` or equivalent in the latest stage will automatically check out the git branches for the earlier stages in a row, and build them one after the other. By time it should be a rare occasion that this needs to be repeated more than once per checkout.
* The build script of stage-n will assume some knowledge of stage-n-1 (i.e. it will refer to files like `../stage-n-1/build/boehm/clasp.exe`, etc)
* Each stage must be buildable using only these:
  * the assumed external toolchain (clang, python, shell, CL for the scraper, etc)
  * the build output of stage n-1
  * the source code found in the git branch of stage-n

## Vision
The current codebase will be branched/duplicated into 4 new branches for the stages, and whatever is not needed will be deleted from them. This will make the early stages much simpler/smaller, and also allow the later stages to assume a much smarter compiler/environment which leads to cleaner code.

Later on patches can be selectively cherry-picked from later stages into earlier stages as needed, e.g. in case an important bug is fixed in the runtime part, or some optimizations may be backported.

Introduction of new stages will be a rare event, and they are independent of clasp versions/releases. A new stage is only needed when we want to use a new feature in the compiler implementation itself.

Examples for new stages:
* We introduce first-class memory spaces, and we want to optimize the compiler by utilizing this feature to optimize GC performance while compiling by creating and throwing away heaps .
* We want to introduce a new generic method caching machinery that also requires support in the runtime (extra complexity in the C++ code).
* We want to write a new GC in CL.

In effect each stage will be similar to a cross compilation from one arch to a completely different arch; i.e. ideally, properly set up algorithms should catch the situations when anything in stage-n is referred to while producing the link artifacts for stage-n+1.

## Open questions

* Would it be possible to eliminate the SBCL dependency by not running the scraper when building the earlier stages (or checking in the scraper output into the repo), and then running the scraper for a later stage using an earlier stage instead of SBCL?
* The stage-n naming convention doesn't accommodate for multiple "ground floors". 

# Building with extensions

## Requiremens for the build infrastructure

The build script of extensions must be able to do at least the following:
* register .cc/.h files for inclusion
* register .lisp files for inclusion
* register link artifacts for the linking of the final exe