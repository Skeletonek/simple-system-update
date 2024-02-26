# Simple System Update

This is a simple script for your Linux distribution to update your packages, and shutdown or reboot your system automaticly. This script supports APT, DNF, Pacman, Flatpak and Snap.

## Instalation

To download and integrate this script with your Linux distribution clone this repository, and put *ssu* file to a directory that is specified in PATH variable. F.e. `/usr/bin` or `/usr/local/bin`. You can put it everywhere else if you don't want the shell to recognize script globally.

To make your instalation easier, make sure you have `git` installed.


```
git clone https://github.com/Skeletonek/simple-system-update.git
sudo mv ./simple-system-update/ssu /usr/local/bin
sudo chmod u+x /usr/local/bin/ssu
rm -rf simple-system-update
```

## Usage

To run script installed by the method shown previously, simply type `sudo ssu` in your terminal, or `ssu` if you are already logged in as root.

After updating all packages, your system will shutdown by default. You can make your system restart after update by using `ssu -r`

You can enable creating a pre-post type system snapshots by using `-b` flag. You need to have Snapper installed and configured.
