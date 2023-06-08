# Labwc-conf

## Overview

Labwc-conf is based on ObConf-Qt which is a Qt port of [ObConf](http://openbox.org/wiki/ObConf:About) and provides some settings for [Labwc](https://labwc.github.io/).

This is early alpha/proof of concept. It needs to be started with ` env QT_QPA_PLATFORM=xcb labwc-conf`.

Most working are already theme, desktops, margins, and font settings.

### To do

- [ ] remove x11 preview code
- [ ] remove openbox dependency
- [ ] set labwc conf directory
- [ ] fix loading translations
- [ ] fix desktop file
- [ ] add/correct settings
- [ ] silence warnings

## Installation

### Compiling source code

Runtime dependencies are Qt X11 Extras, gtk-update-icon-cache, hicolor-icon-theme and Openbox.  
Additional build dependencies are CMake, [liblxqt](https://github.com/lxqt/liblxqt) and [lxqt-build-tools](https://github.com/lxqt/lxqt-build-tools),
optionally Git to pull latest VCS checkouts.

Code configuration is handled by CMake. CMake variable `CMAKE_INSTALL_PREFIX` has to be set to `/usr` on most operating systems.  

To build run `make`, to install `make install` which accepts variable `DESTDIR` as usual.  





