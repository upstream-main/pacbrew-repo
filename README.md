# pacbrew-repo

## Prerequisites
On Debian-flavored operating systems, you can invoke the following commands to
install dependencies used by pacbrew-repo.
```console
john@localhost:pacbrew-repo$ sudo apt-get update && sudo apt-get upgrade \
john@localhost:pacbrew-repo$ sudo apt-get install cmake pkg-config meson clang lld \
                             build-essential autoconf libtool yasm nasm bison flex \
                             gperf pkgconf libarchive-tools autopoint po4a git curl doxygen \
                             makepkg pacman-package-manager python3-mako python3-glad
```

## Building and installing to /opt/ps5-payload-sdk
```console
john@localhost:pacbrew-repo$ export MAKEFLAGS=-j8 # optionally build in parallel on 8 cores
john@localhost:pacbrew-repo$ ./ci-libs.sh
```

