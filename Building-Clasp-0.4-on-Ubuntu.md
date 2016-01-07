###Packages that are necessary to build Clasp on LTS Ubuntu 14.04

Start up VirtualBox 5.0.6 and download Ubuntu 14.04.03 from here:  http://www.ubuntu.com/download/server

Then do the following:

```
sudo apt-get update
sudo apt-get upgrade
```

```
sudo apt-get install --no-install-recommends -y git clang-3.6 clang-3.6-dev llvm-3.6 llvm-3.6-dev libboost-dev libboost-filesystem-dev libboost-date-time-dev libboost-serialization-dev libboost-iostreams-dev libboost-program-options-dev libboost-random-dev libboost-regex-dev libboost-system-dev libgmp-dev autoconf automake libtool libexpat-dev libz-dev libncurses-dev libreadline-dev libedit-dev sbcl

# To clone clasp
git clone https://github.com/drmeister/clasp.git

# To build clasp using 4 processors
```bash
cd clasp
git checkout testing
make clean; PJOBS=4 make
````
# Here they are the dependent libraries broken up into groups.
If you followed the instructions above you don't need this

    sudo apt-get install clang-3.6 clang-3.6-dev llvm-3.6 llvm-3.6-dev -y --no-install-recommends 
    sudo apt-get install libboost-dev libboost-filesystem-dev libboost-date-time-dev libboost-serialization-dev libboost-iostreams-dev libboost-program-options-dev libboost-random-dev libboost-regex-dev libboost-system-dev -y --no-install-recommends 
    sudo apt-get install libgmp-dev -y --no-install-recommends 
    sudo apt-get install autoconf automake libtool -y --no-install-recommends 
    sudo apt-get install libexpat-dev libz-dev libncurses-dev libreadline-dev -y --no-install-recommends
    sudo apt-get install libedit-dev -y --no-install-recommends
    sudo apt-get install sbcl -y --no-install-recommends

    # For development
    sudo apt-get install -y --no-install-recommends emacs