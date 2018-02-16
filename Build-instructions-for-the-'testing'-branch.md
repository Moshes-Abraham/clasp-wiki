# Linux
Adapt paths as necessary.

You may want to look at [this Dockerfile](https://github.com/drmeister/clasp/blob/dev/tools/dockerfiles/cando-build/Dockerfile) that describes how to build on a vanilla Ubuntu 17.10.

1. Debian/Ubuntu: `apt install gcc g++ llvm clang-5.0 libclang-5.0-dev cmake libgc-dev libgmp-dev binutils-gold binutils-dev zlib1g-dev libncurses-dev libboost-filesystem-dev libboost-regex-dev libboost-date-time-dev libboost-program-options-dev libboost-system-dev libboost-iostreams-dev libunwind-dev liblzma-dev`
2. `git clone -b testing https://github.com/drmeister/clasp ~/clasp`
3. `cd ~/clasp`
4. `cp --interactive wscript.config.template wscript.config`

You may need to edit wscript.config at this point.

5. `./waf update_submodules configure build_cboehm`

## Limit resource usage

The build needs a lot of resources, so you may want to build as follows.

Compile in paralel and with low priority:

1. `nice -n 19 ionice --class 3 ./waf build_fboehm`

Then link on a single thread to limit peak memory usage:

2. `nice -n 19 ionice --class 3 ./waf --jobs 1 build_cboehm`
