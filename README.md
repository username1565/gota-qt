# gota-gui

## How to build binaries from source code

### Windows
To build the gui you must have built gota core, so please do all steps from [here](https://github.com/Gotanetwork/gota#building-on-windows) before proceed. Install [QtCreator](https://www.qt.io/download-thank-you?os=windows), open the project file gota-gui/src/gota-gui.pro in QtCreator and build it using MSVS kit (you must have MSVS installed already to build gota core).

### MacOS

To build the gui you must have built gota core, so please do all steps from [here](https://github.com/Gotanetwork/gota#building-on-mac-osx) before proceed. Install [QtCreator](https://www.qt.io/download-thank-you?os=macos), open the project file gota-gui/src/gota-gui.pro in QtCreator and build it using clang kit (you must have XCode installed already to build gota core).

### Linux
```
# To install all required packages on Ubuntu use the following command:
$ sudo apt install qt5-qmake qtbase5-dev qtbase5-dev-tools

$ git clone https://github.com/Gotanetwork/gota.git
$ cd gota
$ mkdir -p build
$ cd build
$ cmake ..
$ make -j4 gota-crypto
$ cd ../..
$ git clone https://github.com/Gotanetwork/gota-gui.git
$ cd gota-gui
$ mkdir -p build
$ cd build
$ cmake ..
$ make -j4
```
Alternative way:
```
# Install QtCreator:
$ sudo apt install qtcreator

$ git clone https://github.com/Gotanetwork/gota.git
$ cd gota
$ mkdir -p build
$ cd build
$ cmake ..
$ make -j4 gota-crypto
$ cd ../..
$ git clone https://github.com/Gotanetwork/gota-gui.git
```
Now open the project file gota-gui/src/gota-gui.pro in QtCreator and build it.
