# Set up an Arch EC2 instance
https://www.uplinklabs.net/projects/arch-linux-on-ec2/

I used the m4.large with 24Gb Disk space

# Set up a user and log in

useradd -m -G wheel -s /bin/bash meister
su - meister

# Download packages
```
sudo pacman -S emacs
sudo pacman -S git
sudo pacman -S cmake
```
