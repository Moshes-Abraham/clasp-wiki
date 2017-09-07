# Linux
Adapt paths as necessary. 

1. Debian/Ubuntu: `apt install gcc g++ llvm clang cmake libgc-dev libgmp-dev binutils-gold binutils-dev zlib1g-dev libncurses-dev libboost-filesystem-dev libboost-regex-dev libboost-date-time-dev libboost-program-options-dev libboost-system-dev libboost-iostreams-dev`
2. `git clone -b master https://github.com/drmeister/externals-clasp ~/externals-clasp`
3. `git clone -b testing https://github.com/drmeister/clasp ~/clasp`
4. `cd ~/externals-clasp && make`
5. `cd ~/clasp && echo "EXTERNALS_CLASP_DIR = '$HOME/externals-clasp'" > wscript.config`
6. `./waf configure update_submodules build_cboehm`

# OS X
You'll need XCode and Homebrew for some of the extra packages that are needed to build everything. Otherwise things are much the same as on the Linux side -- hopefully. Adapt paths as necessary.

1. `brew install gmp bdw-gc cmake boost`
2. `git clone https://github.com/drmeister/externals-clasp ~/externals-clasp`
3. `git clone https://github.com/drmeister/clasp ~/clasp`
4. `cd ~/externals-clasp && make`
5. `cd ~/clasp && echo "EXTERNALS_CLASP_DIR = '$HOME/externals-clasp'" > wscript.config`
6. `./waf configure update_submodules build_cboehm`

If you get compiler errors on the first try, then the open source clang may need to be informed where the OS X compiler resources (header files) are located.

### Informing clang about the Xcode resource path
#### These instructions worked most recently on Sep 6, 2017 (drmeister) - although we had to edit the paths a little.

#### We installed gmp using home-brew.
7. `mv ~/externals-clasp/build/release/include/c++/v1 ~/externals-clasp/build/release/include/c++/v1-original`
8. `ln -s /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1 ~/externals-clasp/build/release/include/c++/v1`

Note: The Xcode path may change from time to time when OS X/Xcode releases are made.

If there are still problems - try reinstalling Xcode command line tools:     `xcode-select --install`