# Install the required libraries
I use "brew"

    brew install gmp
    brew install boost155

Compile llvm3.6/clang in a local directory - on my system the include files end up in:
/Users/meister/Development/externals-clasp/build/release/include

# Settings for linux

## Edit the clasp/local.config
    export CLASP_CXXFLAGS = -I/home/meister/Development/externals-clasp/build/release/include
    export CLASP_CXXFLAGS += -I/home/meister/Development/externals-clasp/build/common/include
    export CLASP_LINKFLAGS = "-L/home/meister/Development/externals-clasp/build/release/lib"
    export CLASP_LINKFLAGS += "-L/home/meister/Development/externals-clasp/build/common/lib"
    export CLASP_LINKFLAGS += "-L/home/meister/.local/lib"

    export CLANG_BIN_DIR="/home/meister/Development/externals-clasp/build/release/bin"

    export LINK = shared

LINK can also be set to static