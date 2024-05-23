# Appcons Theme

![Obsidian App Icon](./apps/128/obsidian.svg)
![Alacritty App Icon](./apps/128/alacritty.svg)

A collection of vector icons for popular applications that strives to better mesh with the visual language of elementary OS.
This theme is designed to be installed on top of and extend the regular [icons theme](https://github.com/elementary/icons) for elementary OS.


<img src="https://github.com/wpkelso/appcons/assets/11094688/5c8fb765-61c3-4f79-a33d-46b5bd59c480" width="200">

_designed for elementary OS_

## Building and Installation

You'll need the following dependencies:

* meson
* rsvg

Run `meson` to configure the build environment and then `ninja` to build

    meson build --prefix=/usr
    cd build
    ninja

To install, use `ninja install`

    sudo ninja install
