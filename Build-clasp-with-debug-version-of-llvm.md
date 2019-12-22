Clone llvm-project from github.

Build llvm with this...

cd llvm-project
mkdir build
cd build
cmake -DLLVM_BUILD_LLVM_DYLIB=true -DLLVM_ENABLE_PROJECTS=clang -G "Unix Makefiles" ../llvm 
make -j<pids>



