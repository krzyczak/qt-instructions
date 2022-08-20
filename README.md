# QT / QML Instructions

There are the following three repositories:
- https://github.com/AsteroidOS/asteroid-launcher (compiled with qmake and make)
- https://github.com/nemomobile-ux/glacier-home (compiled with cmak and make; more details: https://nemomobile.net/glacier-home/)
- https://github.com/nemomobile-graveyard/lipstick-example-home

The asteroid-launcher is based on glacier-home, which is based on lipstick (https://github.com/sailfishos/lipstick/) and wayland.

All of these can run on the postmarketOS (https://postmarketos.org/) and in fact are already bundled.

I want to be able to modify them and cross-compile and run on a device running the postmarketOS base version without any UI installed.

### Assumtions
1. There is a machine with a fresh ubuntu installation
2. There is a modile device running postmarketOS with the none/console UI as shown here: https://wiki.postmarketos.org/wiki/Category:Interface

### Task
The task is to create an MD file with a step by step instructions, describing:
1. Which packages need to be installed on ubuntu with detailed description on how to install them.

   For examlple if a `build-essential` or `cmake` package is required the MD file should say:

   > Next install the `cmake` and `build-essential` packages with the following command:
   > ```bash
   >   sudo apt-get install -y build-essential cmake
   > ```
   
   It could also briefly describe what does each package do.
   
2. Which dependencies need to be downloaded or cloned (with links) and compiled and installed, with detailed description of how to compile them.
   
   For example if a dependency needs to be compiled manually the MD file should say:
   > Next download, compile and install the `example` package:
   > ```bash
   >   git clone https://www.example.org/example.git
   >   cd example
   >   cmake .
   >   make
   >   make install
   > ```
   
3. Detailed description on how to cross-compile each of the apps (asteroid-launcher, glacier-home, lipstick-example-home) and how to deploy and run them on the mobile device running the postmarketOS.

