# Simple System Update

This is a simple script for your Linux distribution to update your packages, and shutdown or reboot your system automaticly. This script supports APT, DNF, Pacman, Flatpak and Snap.

## Instalation

To download and integrate this script with your Linux distribution clone this repository, and put *ssu* file to `$HOME/.local/bin` or `/usr/bin` or `/usr/local/bin`. Moving it to `$HOME/.local/bin` will show script only for one user.

To make your instalation easier, make sure you have `git` installed.

This will install script for current user:

```
git clone https://github.com/Skeletonek/simple-system-update.git
mv ./simple-system-update/ssu ~/.local/bin/
chmod u+x ~/.local/bin/ssu
rm -rf simple-system-update
```

This will install script system-wide, but you need to be logged in as root:

```
git clone https://github.com/Skeletonek/simple-system-update.git
mv ./simple-system-update/ssu /usr/local/bin
chmod u+x /usr/local/bin/ssu
rm -rf simple-system-update
```

## Usage

To run script installed by the method shown previously, simply type `ssu` in your terminal. **Your system will probably ask you for sudo password.**

After updating all packages, your system will shutdown by default. You can make your system restart after update by using `ssu -r`
