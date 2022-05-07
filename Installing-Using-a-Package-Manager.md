Work is in progress to enable build and installing Clasp/Cando from package managers such as apt-get, brew, etc. Currently, the only supported package is the Arch AUR package. If you are using MacOS or a non-Arch based Linux distribution you will need to build Clasp/Cando from source.

# Installing on Arch using a AUR helper

Installing Clasp on Arch can be done using an AUR helper such as [yay](https://github.com/Jguer/yay). Building in this manner using
the [clasp-cl-git](https://aur.archlinux.org/packages/clasp-cl-git/) package will build both Clasp and Cando and will install all
dependencies as needed. If you do not have yay installed you can install via the following commands.

```
pacman -S --needed git base-devel
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

Once yay is installed you can installation Clasp with `yay clasp-cl-git`.