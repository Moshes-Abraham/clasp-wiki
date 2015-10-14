###Packages that are necessary to install Clasp on LTS Ubuntu 14.04.3

    sudo apt-get update
    sudo apt-get upgrade

    sudo apt-get git

    git clone https://github.com/drmeister/clasp.git

clang-3.6 clang-3.6-dev llvm-3.6 llvm-3.6-dev

apt-get install --no-install-recommends clang-3.6 clang-3.6-dev llvm-3.6 llvm-3.6-dev
;; Boost
apt-get install --no-install-recommends libboost-dev libboost-filesystem-dev libboost-date-time-dev libboost-serialization-dev libboost-iostreams-dev libboost-program-options-dev libboost-random-dev libboost-regex-dev libboost-system-dev
;; Gmp
apt-get install --no-install-recommends libgmp-dev
;; Boehm
apt-get install --no-install-recommends autoconf automake libtool
;; Deps
apt-get install --no-install-recommends libexpat-dev libz-dev libncurses-dev libreadline-dev