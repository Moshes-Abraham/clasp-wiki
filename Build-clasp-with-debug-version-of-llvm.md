Clone llvm-project from github.

Build llvm with this...

cd llvm-project
mkdir build
cd build
cmake -DLLVM_BUILD_LLVM_DYLIB=true -DLLVM_ENABLE_PROJECTS=clang -G "Unix Makefiles" ../llvm 
make -j<pids>


Maybe better to build llvm with this...
all:
	(cd build; cmake -G "Unix Makefiles" \
	-DLIBOMP_ARCH=x86_64
	-DLINK_POLLY_INTO_TOOLS=ON
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
	-DFFI_INCLUDE_DIR=/usr/local/Cellar/libffi/3.2.1/lib/libffi-3.2.1/include \
	-DFFI_LIBRARY_DIR=/usr/local/Cellar/libffi/3.2.1/lib \
	-DLLVM_CREATE_XCODE_TOOLCHAIN=ON \
	-DLLDB_USE_SYSTEM_DEBUGSERVER=ON \
	-DLLDB_DISABLE_PYTHON=1 \
	-DLIBOMP_INSTALL_ALIASES=OFF )




