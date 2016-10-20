# Linux
Adapt paths as necessary. Required prerequisites are: a sane compiler environment for C and C++, boehmgc, cmake, boost of recent enough versions. Debian stable unfortunately does not yet sport high enough versions of the latter two.

1. `git clone https://github.com/drmeister/externals-clasp ~/externals-clasp`
2. `git clone https://github.com/drmeister/clasp ~/clasp`
3. `cd ~/externals-clasp && make`
4. `cd ~/clasp && echo "EXTERNALS_CLASP_DIR = '$HOME/externals-clasp'" > local.config`
5. `make`

# OS X

1. `brew install bdw-gc cmake boost`
2. `git clone https://github.com/drmeister/externals-clasp ~/externals-clasp`
3. `git clone https://github.com/drmeister/clasp ~/clasp`
4. `cd ~/externals-clasp && make`
5. `cd ~/clasp && echo "EXTERNALS_CLASP_DIR = '$HOME/externals-clasp'" > local.config`
6. `make`

## The following is old set up information that I may or may not need to move up into the instructions
The open source clang may need to be informed where the OS X compiler resources (header files) are located.

So the following symbolic link needs to be installed.

Let's say the external clang executable is installed at `/Users/meister/Development/externals-clasp/build/release/bin/clang`.

Then use:  

     $ mv /Users/meister/Development/externals-clasp/build/release/include/c++/v1 /Users/meister/Development/externals-clasp/build/release/include/c++/v1-original  
     $ ln -s /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1 /Users/meister/Development/externals-clasp/build/release/include/c++/v1

Note: The path `/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1` may change from time to time when OS X/Xcode releases are made.
