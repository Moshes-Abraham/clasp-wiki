Building Clasp on OS X requires using the same version of Clang that Clasp is linked with.  I use the llvm/clang version that gets built by externals-clasp.

This clang needs to be informed where OS X compiler resources (header files) are located.

So the following symbolic link needs to be installed.

Let's say the external clang executable is installed at /Users/meister/Development/externals-clasp/build/release/bin/clang.

Then use:  
     $ mv /Users/meister/Development/externals-clasp/build/release/include/c++/v1 /Users/meister/Development/externals-clasp/build/release/include/c++/v1-original  
     $ ln -s /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1 /Users/meister/Development/externals-clasp/build/release/include/c++/v1

Note: The path /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/include/c++/v1 may change from time to time when OS X/Xcode releases are made.
