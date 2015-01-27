# Installation

## clone patches repository including the dwm repository

    git clone https://github.com/jceb/dmenu-patches

## init and load dwm submodule

    cd dmenu-patches
    git submodule update --init --recursive

## activate all patches, including the personal configuration

    quilt push -a

## build st (or us the ./build script)

    cd dmenu
    rm -f config.h
    make

## install st locally (or use ./install script)

    make DESTDIR=~/.local PREFIX= install

# Patch References

* [fuzzymatch.patch](patches/fuzzymatch.patch)   (http://tools.suckless.org/dmenu/patches/fuzzymatch)
