Clone llvm-project from github.

Build llvm with this...

cd llvm-project
mkdir build
cd build
cmake -DLLVM_BUILD_LLVM_DYLIB=true -DLLVM_ENABLE_PROJECTS=clang -G "Unix Makefiles" ../llvm 
make -j<pids>

Lots of stuff is missing when linking ...


Maybe better to build llvm with this...
```
(cd build; cmake -G "Unix Makefiles" 
	-DLLVM_BUILD_EXTERNAL_COMPILER_RT=ON 
	-DLLVM_BUILD_LLVM_DYLIB=ON 
	-DLLVM_ENABLE_EH=ON 
	-DLLVM_ENABLE_LIBCXX=ON 
	-DLLVM_ENABLE_RTTI=ON 
	-DLLVM_INCLUDE_DOCS=OFF 
	-DLLVM_INSTALL_UTILS=ON 
	-DLLVM_OPTIMIZED_TABLEGEN=ON 
	-DLLVM_TARGETS_TO_BUILD=all 
         -DLLVM_ENABLE_PROJECTS=clang ../llvm )
```



