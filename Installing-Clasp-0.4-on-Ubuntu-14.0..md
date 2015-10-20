###Packages that are necessary to install Clasp on LTS Ubuntu 14.04.3

Start up VirtualBox 5.0.6 and download Ubuntu 14.04.03 from here:  http://www.ubuntu.com/download/server

Then do the following:

    sudo apt-get update
    sudo apt-get upgrade

    sudo apt-get install --no-install-recommends -y git clang-3.6 clang-3.6-dev llvm-3.6 llvm-3.6-dev libboost-dev libboost-filesystem-dev libboost-date-time-dev libboost-serialization-dev libboost-iostreams-dev libboost-program-options-dev libboost-random-dev libboost-regex-dev libboost-system-dev libgmp-dev autoconf automake libtool libexpat-dev libz-dev libncurses-dev libreadline-dev libedit-dev

    # To clone clasp
    git clone https://github.com/drmeister/clasp.git

    # To build clasp using 4 processors
    cd clasp
    git checkout testing
    make clean; PJOBS=4 make

# Here they are the dependent libraries broken up into groups.
If you followed the instructions above you don't need this

    sudo apt-get install -y --no-install-recommends clang-3.6 clang-3.6-dev llvm-3.6 llvm-3.6-dev
    sudo apt-get install -y --no-install-recommends libboost-dev libboost-filesystem-dev libboost-date-time-dev libboost-serialization-dev libboost-iostreams-dev libboost-program-options-dev libboost-random-dev libboost-regex-dev libboost-system-dev
    sudo apt-get install -y --no-install-recommends libgmp-dev
    sudo apt-get install -y --no-install-recommends autoconf automake libtool
    sudo apt-get install -y --no-install-recommends libexpat-dev libz-dev libncurses-dev libreadline-dev
    sudo apt-get install -y --no-install-recommends libedit-dev

    # Run them all as one big apt-get

    # For development
    sudo apt-get install -y --no-install-recommends emacs