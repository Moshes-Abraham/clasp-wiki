# Linux
Adapt paths as necessary. 

1. Debian/Ubuntu: `apt install gcc g++ llvm clang cmake libgc-dev libgmp-dev binutils-gold binutils-dev zlib1g-dev libncurses-dev libboost-filesystem-dev libboost-regex-dev libboost-date-time-dev libboost-program-options-dev libboost-system-dev libboost-iostreams-dev`
2. `git clone -b master https://github.com/drmeister/externals-clasp ~/externals-clasp`
3. `git clone -b testing https://github.com/drmeister/clasp ~/clasp`
4. `cd ~/externals-clasp && make`
5. `cd ~/clasp && echo "LLVM_CONFIG_BINARY = '$HOME/externals-clasp/build/release/bin/llvm-config'" > wscript.config`
6. `./waf update_submodules configure build_cboehm`

# OS X
You'll need XCode and Homebrew for some of the extra packages that are needed to build everything. Otherwise things are much the same as on the Linux side -- hopefully. Adapt paths as necessary.

## Install externals-clasp until the builtin Xcode can build clasp (Xcode could not as of Sep 6, 2017)
1. `git clone https://github.com/drmeister/externals-clasp ~/externals-clasp`
2. `cd ~/externals-clasp && make`

#### Informing the new clang about the Xcode resource path
#### These instructions worked most recently on Sep 6, 2017 (drmeister) 

3. `mv ~/externals-clasp/build/release/include/c++/v1 ~/externals-clasp/build/release/include/c++/v1-original`
4. `ln -s /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1 ~/externals-clasp/build/release/include/c++/v1`

Note: The Xcode path may change from time to time when OS X/Xcode releases are made.

5. `brew install gmp bdw-gc cmake boost libunwind-headers`
6. `git clone https://github.com/drmeister/clasp ~/clasp`
7. `cd ~/clasp && echo "LLVM_CONFIG_BINARY = '$HOME/externals-clasp/build/release/bin/llvm-config'" > wscript.config`
8. `./waf update_submodules configure build_cboehm`

If there are still problems - try reinstalling Xcode command line tools and start again.

Use:     `xcode-select --install`