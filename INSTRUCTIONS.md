# Installing dependencies for QT / QML wayland based home launcher for postmarketOS (and other linux distributions).

This file describes how to install dependencies for for the [asteroid-launcher](https://github.com/AsteroidOS/asteroid-launcher), [glacier-home](https://github.com/nemomobile-ux/glacier-home) and [lipstick-example-home](https://github.com/nemomobile-graveyard/lipstick-example-home) projects and how to compile and run them.

# Dependencies
Starting with a fresh ubuntu installation the first package required is build-essential. This package is a reference for all the packages needed to compile a package on a debian based linux distribution. It generally includes the GCC/g++ compilers and libraries and some other utilities. To install it runn the following command:
```bash
sudo apt-get install -y build-essential cmake
```

...
