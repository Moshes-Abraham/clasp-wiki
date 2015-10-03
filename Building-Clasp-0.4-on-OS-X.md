# Install the required libraries
I use "brew"

brew install gmp
brew install boost155

Compile llvm3.6/clang in a local directory - on my system the include files end up in:
/Users/meister/Development/externals-clasp/build/release/include

## Edit the clasp/local.config
    export CLASP_CXXFLAGS = -I/usr/local/opt/boost155/include
    export CLASP_CXXFLAGS += -I/usr/local/Cellar/gmp/6.0.0a/include
    export CLASP_CXXFLAGS += -I/Users/meister/Development/externals-clasp/build/release/include
    export CLASP_LINKFLAGS = "-L/usr/local/opt/boost155/lib"

