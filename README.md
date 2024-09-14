# Appcons Theme

![Obsidian](./apps/64/obsidian.svg)
![Alacritty](./apps/64/com.alacritty.Alacritty.svg)
![Inkscape](./apps/64/org.inkscape.Inkscape.svg)
![Zen Browser](./apps/64/io.github.zen_browser.zen.svg)

A small but growing collection of vector icons for third-party applications that strives to better mesh with the visual language of elementary OS.
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
