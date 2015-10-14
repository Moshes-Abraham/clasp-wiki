###Packages that are necessary to install Clasp on LTS Ubuntu 14.04.3

    sudo apt-get update
    sudo apt-get upgrade

    sudo apt-get git --no-install-recommends -y

    sudo apt-get install clang-3.6 clang-3.6-dev llvm-3.6 llvm-3.6-dev --no-install-recommends -y

    # Boost
    sudo apt-get install libboost-dev libboost-filesystem-dev libboost-date-time-dev libboost-serialization-dev libboost-iostreams-dev libboost-program-options-dev libboost-random-dev libboost-regex-dev libboost-system-dev -y --no-install-recommends
    # Gmp
    sudo apt-get install -y --no-install-recommends libgmp-dev
    # For building Boehm
    sudo apt-get install -y --no-install-recommends autoconf automake libtool
    # Other dependent libraries
    sudo apt-get install -y --no-install-recommends libexpat-dev libz-dev libncurses-dev libreadline-dev

    # Finally, to clone clasp
    git clone https://github.com/drmeister/clasp.git
