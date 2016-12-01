# Linux
Adapt paths as necessary. 

1. Install `gcc g++ boehmgc cmake boost`
2. `git clone -b master https://github.com/drmeister/externals-clasp ~/externals-clasp`
3. `git clone -b testing https://github.com/drmeister/clasp ~/clasp`
4. `cd ~/externals-clasp && make`
5. `cd ~/clasp && echo "EXTERNALS_CLASP_DIR = '$HOME/externals-clasp'" > wscript.config`
6. `./waf configure update_submodules build_cboehm`

# OS X
You'll need XCode and Homebrew for some of the extra packages that are needed to build everything. Otherwise things are much the same as on the Linux side -- hopefully. Adapt paths as necessary.

1. `brew install bdw-gc cmake boost`
2. `git clone https://github.com/drmeister/externals-clasp ~/externals-clasp`
3. `git clone https://github.com/drmeister/clasp ~/clasp`
4. `cd ~/externals-clasp && make`
5. `cd ~/clasp && echo "EXTERNALS_CLASP_DIR = '$HOME/externals-clasp'" > wscript.config`
6. `./waf configure update_submodules build_cboehm`

If you get compiler errors on the first try, then the open source clang may need to be informed where the OS X compiler resources (header files) are located.

### Informing clang about the Xcode resource path
7. `mv ~/externals-clasp/build/release/include/c++/v1 ~/externals-clasp/build/release/include/c++/v1-original`
8. `ln -s /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1 ~/externals-clasp/build/release/include/c++/v1`

Note: The Xcode path may change from time to time when OS X/Xcode releases are made.
