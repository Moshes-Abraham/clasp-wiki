# Linux
In Linux I installed from scratch on top of Ubuntu 18.04 LTS and Ubuntu 20.14.

Install the following packages:
* Install llvm@9 (see http://apt.llvm.org/ Install(old-stable branch)
  * LLVM
`sudo apt-get install libllvm-9-ocaml-dev libllvm9 llvm-9 llvm-9-dev llvm-9-doc llvm-9-examples llvm-9-runtime`
  * Clang and co
`sudo apt-get install clang-9 clang-tools-9 clang-9-doc libclang-common-9-dev libclang-9-dev libclang1-9 clang-format-9 python-clang-9 clangd-9`
  * lldb
`sudo apt-get install lldb-9`
  * lld (linker)
`sudo apt-get install lld-9`
  * libc++ `sudo apt-get install libc++-9-dev libc++abi-9-dev`

or minimal:
* `sudo apt-get install libllvm9 llvm-9 llvm-9-dev llvm-9-runtime`
* `sudo apt-get install clang-9 clang-tools-9 libclang-common-9-dev libclang-9-dev libclang1-9 clang-format-9 clangd-9`
* `sudo apt-get install lldb-9`
* `sudo apt-get install lld-9`
* `sudo apt-get install libc++-9-dev libc++abi-9-dev`

and 
* `sudo apt-get -y install curl git gpg libboost-date-time-dev` 
* `sudo apt-get install libboost-filesystem-dev libboost-graph-dev libboost-iostreams-dev`
* `sudo apt-get install libboost-program-options-dev libboost-regex-dev libboost-system-dev`
* `sudo apt-get install libbsd-dev libelf-dev libexpat-dev libgmp-dev`
* `sudo apt-get install libzmq3-dev nano npm python3-pip sbcl wget zlib1g-dev libunwind-dev`

* perhaps `sudo apt install libncurses-dev libelf1 python2`
* install bdw-gc from https://github.com/clasp-developers/clasp-boehm (should the process complain that it can't find a makefile, put `make -C $(GC) -f Makefile install` instead of `make -C $(GC) -f makefile install` in the makefile
* `git clone https://github.com/clasp-developers/clasp.git`
* `git checkout master`
* `cp wscript.config.debian10 wscript.config`
* edit in wscript.config setting LLVM_CONFIG_BINARY = '/path/to/llvm-config-4.0' to the corrrect path, in my case /usr/bin/llvm-config-9
* add `INCLUDES = [ "-I", "/lib/llvm-9/include/c++/v1"]`to wscript.conf
* install emacs `sudo snap install emacs --classic`
* `./waf distclean configure build_cboehm` (can take 1-2 hours)
* Start with `build/clasp`

# MacOSX Catalina/Mojave
* install xcode
* install xcode command line tools
* install sbcl
* brew install llvm@9
* brew install cmake libffi gmp boost libunwind-headers
* install bdw-gc from https://github.com/clasp-developers/clasp-boehm (should the process complain that it can't find a makefile, put `make -C $(GC) -f Makefile install` instead of `make -C $(GC) -f makefile install` in the makefile
* `git clone https://github.com/clasp-developers/clasp.git`
* `git checkout dev`
* `cp wscript.config.osx-brew wscript.config`
* adapt wscript.config
  * change LLVM_CONFIG_BINARY to the correct path, in my case
`LLVM_CONFIG_BINARY = '/usr/local/opt/llvm@9/bin/llvm-config'`
  * add the following two settings (this assumes, you have the command line tools installed)
```c++
CPPFLAGS = [ "-Wno-nullability-completeness"]
INCLUDES = [ "-I", "/Library/Developer/CommandLineTools/usr/include/c++/v1",
             "-I", "/Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/include"
]
````
* for catalina add additionally
```c++
CPPFLAGS = [ "-isystem", "/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX10.15.sdk"]
````
  * My complete wscript.config is the following
```c++
#LLVM_CONFIG_BINARY = '/usr/local/opt/llvm@6/bin/llvm-config'
LLVM_CONFIG_BINARY = '/usr/local/opt/llvm@9/bin/llvm-config'
USE_PARALLEL_BUILD = True
USE_BUILD_FORK_REDIRECT_OUTPUT = False
CLASP_BUILD_MODE = 'object'
USE_COMPILE_FILE_PARALLEL = False
DEBUG_OPTIONS = [  "DEBUG_RELEASE"
                  ,"DEBUG_BCLASP_LISP"
                  ,"DEBUG_CCLASP_LISP"
                  ,"DEBUG_COMPILER"
                  ,"DEBUG_GUARD"
                  ,"DEBUG_GUARD_VALIDATE"
                  ,"DEBUG_ASSERT_TYPE_CAST"
                  ,"DEBUG_VERIFY_MODULES"
                  ,"CST"
                  ]
REQUIRE_LIBFFI = True
CPPFLAGS = [ "-Wno-nullability-completeness"]
INCLUDES = [ "-I", "/Library/Developer/CommandLineTools/usr/include/c++/v1",
             "-I", "/Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/include"
]
````
* to build from scratch  `./waf distclean configure build_cboehm`, can take 1 hour
* to verify build `./waf test`
* Start with `build/clasp`
* to install `./waf install_cboehm`
# Known errors
* ~~Disassemble no longer works~~
* ~~cl:format no longer works correctly~~
* ~~Backtraces in slime or in terminal with (core:btcl) or with (core:safe-backtrace) are slightly broken~~
# what you want to do on top
* update sbcl (remember you need a valid common lisp (e.g. sbcl) to update sbcl, see see http://www.sbcl.org/platform-table.html
* install slime
* install quicklisp, see https://www.quicklisp.org/beta/#installation