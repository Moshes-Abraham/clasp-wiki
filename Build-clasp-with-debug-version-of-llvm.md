# On Linux/Debian

The ld.gold linker needs to be available.  I don't know if /bin/ld.gold is all you need so I moved /bin/ld to /bin/ld.orig and created a symlink from /bin/ld.gold to /bin/ld

Install binutils-dev
```
sudo apt-get install binutils-dev
```

Clone llvm-project from github.

Build llvm with this in a makefile in llvm-projects ...


```
all:
        (cd build; cmake -G "Unix Makefiles" \
        -DLIBOMP_ARCH=x86_64 \
        -DLLVM_BINUTILS_INCDIR=/usr/include \
        -DLLVM_ABI_BREAKING_CHECKS=FORCE_OFF \
        -DLINK_POLLY_INTO_TOOLS=ON \
        -DLLVM_BUILD_EXTERNAL_COMPILER_RT=ON \
        -DLLVM_BUILD_LLVM_DYLIB=ON \
        -DLLVM_ENABLE_ASSERTIONS=ON \
        -DLLVM_ENABLE_EH=ON \
        -DLLVM_ENABLE_FFI=ON \
        -DLLVM_ENABLE_LIBCXX=ON \
        -DLLVM_ENABLE_RTTI=ON \
        -DLLVM_INCLUDE_DOCS=OFF \
        -DLLVM_INSTALL_UTILS=ON \
        -DLLVM_OPTIMIZED_TABLEGEN=ON \
        -DLLVM_TARGETS_TO_BUILD=all \
        -DLLVM_ENABLE_PROJECTS=clang \
        -DCMAKE_BUILD_TYPE=RelWithDebInfo \
        -DWITH_POLLY=ON \
        -DLLDB_USE_SYSTEM_DEBUGSERVER=ON \
        -DLLDB_DISABLE_PYTHON=1 \
        -DLIBOMP_INSTALL_ALIASES=OFF ../llvm )

```
```
cd llvm-project
mkdir build
make
```
Add this to the wscript.config

```
LLVM_CONFIG_BINARY = '<path-to-llvm-project>/build/bin/llvm-config'
INCLUDES = ["<path-to-llvm-project>/clang/include", "<path-to-llvm-project>/build/tools/clang/include"]
```



# On MacOS

Clone llvm-project from github.

Build llvm with this...

cd llvm-project
mkdir build

I don't know which of the following worked in the end so figure out which one and then remove the other from these instructions.

1.

Copy this into makefile and run.
```

all:
	(cd build; cmake -G "Unix Makefiles" \
	-DLIBOMP_ARCH=x86_64 \
	-DLLVM_ABI_BREAKING_CHECKS=FORCE_OFF \
	-DLINK_POLLY_INTO_TOOLS=ON \
	-DLLVM_BUILD_EXTERNAL_COMPILER_RT=ON \
	-DLLVM_BUILD_LLVM_DYLIB=ON \
	-DLLVM_ENABLE_EH=ON \
	-DLLVM_ENABLE_FFI=ON \
	-DLLVM_ENABLE_LIBCXX=ON \
	-DLLVM_ENABLE_RTTI=ON \
	-DLLVM_INCLUDE_DOCS=OFF \
	-DLLVM_INSTALL_UTILS=ON \
	-DLLVM_OPTIMIZED_TABLEGEN=ON \
	-DLLVM_TARGETS_TO_BUILD=all \
	-DLLVM_ENABLE_PROJECTS=clang \
	-DCMAKE_BUILD_TYPE=RelWithDebInfo \
	-DWITH_POLLY=ON \
	-DFFI_INCLUDE_DIR=/usr/local/Cellar/libffi/3.2.1/lib/libffi-3.2.1/include \
	-DFFI_LIBRARY_DIR=/usr/local/Cellar/libffi/3.2.1/lib \
	-DLLVM_CREATE_XCODE_TOOLCHAIN=ON \
	-DLLDB_USE_SYSTEM_DEBUGSERVER=ON \
	-DLLDB_DISABLE_PYTHON=1 \
	-DLIBOMP_INSTALL_ALIASES=OFF ../llvm )

```
### OR copy this into run-cmake and run it
 ```
cmake -G "Unix Makefiles" ../llvm \
-DCMAKE_C_FLAGS_RELEASE=-DNDEBUG \
-DCMAKE_CXX_FLAGS_RELEASE=-DNDEBUG \
-DCMAKE_INSTALL_PREFIX=/usr/local/Cellar/llvm/9.0.0_1 \
-DCMAKE_FIND_FRAMEWORK=LAST \
-DCMAKE_VERBOSE_MAKEFILE=ON \
-Wno-dev \
-DCMAKE_BUILD_TYPE=RelWithDebInfo \
-DLIBOMP_ARCH=x86_64 \
-DLINK_POLLY_INTO_TOOLS=ON \
-DLLVM_BUILD_EXTERNAL_COMPILER_RT=ON \
-DLLVM_BUILD_LLVM_DYLIB=ON \
-DLLVM_ENABLE_EH=ON \
-DLLVM_ENABLE_FFI=ON \
-DLLVM_ENABLE_LIBCXX=ON \
-DLLVM_ENABLE_RTTI=ON \
-DLLVM_INCLUDE_DOCS=OFF \
-DLLVM_INSTALL_UTILS=ON \
-DLLVM_OPTIMIZED_TABLEGEN=ON \
-DLLVM_TARGETS_TO_BUILD=all \
-DWITH_POLLY=ON \
-DFFI_INCLUDE_DIR=/usr/local/opt/libffi/lib/libffi-3.2.1/include \
-DFFI_LIBRARY_DIR=/usr/local/opt/libffi/lib \
-DLLVM_CREATE_XCODE_TOOLCHAIN=ON \
-DLLDB_USE_SYSTEM_DEBUGSERVER=ON \
-DLLDB_DISABLE_PYTHON=1 \
-DLIBOMP_INSTALL_ALIASES=OFF \
-DLLVM_ENABLE_PROJECTS=clang

```

Then edit wscript.config and add these options...


```
LLVM_CONFIG_BINARY = '/Users/meister/Development/llvm-project/build/bin/llvm-config'
CPPFLAGS = [ "-isystem", "/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1", "-I", "/Users/meister/Development/llvm-project/build/include", "-I", "/Users/meister/Development/llvm-project/build/tools/clang/include", "-I", "/Users/meister/Development/llvm-project/clang/include", "-Wno-nullability-completeness", "-Wno-nonnull"]

#"--sysroot", "/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX.sdk",
```

NOTE: DO NOT USE THE --sysroot option - that messes up math includes - I don't know why.
I put it here so that we might figure out why it messes things up.


Then build with:

./waf build_iboehm

### Then:

```
install_name_tool -add_rpath $HOME/Development/llvm-project/build/lib build/boehm/iclasp-boehm 
```

### Then:

./waf build_aboehm -v
