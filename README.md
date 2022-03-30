# archpkg
PKGBUILDs and a package repository for Archlinux (x86_64 and aarch64)

Few PKGBUILDs with the main intent to provide a PKGBUILD for `linux-aarch64-rpi`, a kernel package for generic Archlinux ARM aarch64 installs with all drivers and additions from the raspberrypi-linux kernel tree, based on the official `linux-aarch64` and `linux-rpi` packages.

Binary packages (x86_64, aarch64) plus repository metadata are provided aswell, containing a few more packages built from official AUR (for easier installation and to save build time).

## How to install and use the repository

Note: Neither the packages nor the repository are signed!

Add to /etc/pacman.conf:
```
[herrnst-archpkg]
SigLevel = Optional TrustAll
Server = https://raw.githubusercontent.com/herrnst/archpkg/master/packages/$arch/
```
