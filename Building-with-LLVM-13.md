* Install ubuntu 20.10
* sudo apt install sbcl
* sudo apt-get install git make build-essential curl
* sudo apt install libboost-filesystem-dev libboost-graph-dev libboost-regex-dev libboost-date-time-dev libboost-program-options-dev libboost-system-dev libboost-iostreams-dev
* sudo apt-get libgmp-dev libffi-dev zlib1g-dev libelf-dev libncurses-dev libbsd-dev
* convenience
  * sudo apt-get install emacs
* Get llvm 13 by
  * download https://github.com/yitzchak/mpr/releases/tag/llvm13_13.r5140.g972b6a3a3471-1
  * sudo apt-get install 'the download from above´
  * is installed in `/opt/llvm13`
* or use a packaged boehm
* GC
  * git clone https://github.com/clasp-developers/clasp-boehm
  * Fix the error in the Makefile (in rule build Makefile instead of makefile
  * sudo make
  * goes to `opt/clasp-support`
* Alternatively to the previous step, use a prepackaged boehm
* Clasp
  * git clone https://github.com/clasp-developers/clasp.git
  * cp wscript.config.debian10 wscript.config
  * in wscript edit llvm_config_binary to `/opt/llvm13/bin/llvm-config`
  * For Boehmgc self compiled add `INCLUDES = ["/opt/clasp-support/include"]` and `LINKFLAGS = ["-L/opt/clasp-support/lib"]`
* assure python version 3.7.x or earlier installed
  * if python 3.8.x installed, follow http://codingadventures.org/2020/08/30/how-to-install-pyenv-in-ubuntu/ and install and set python 3.7.x
  * to compie python 3.7.x, I needed `sudo apt-get install make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev`

* build clasp
   * `./waf distclean`
   * `./waf configure`
   * `./waf build_dboehmprecise` might take hours

* if configure complains about an sbcl not recent enough, put the following in wscript (instead of 2.1)
````
SBCL_VERSION = (2, 0)
SBCL_VERSION_STRING = "2.0"
````