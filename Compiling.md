Dependencies
============

- Qt 5 >= 5.0 (`qt5-qtbase-devel` and `qt5-qttools` in Fedora, `qtbase5-dev` and `qt5-qmake` in Debian/Ubuntu)
- Botan >= 1.10 (`botan-devel` in Fedora, `libbotan1.10-dev` in Debian/Ubuntu)
- A C++ Compiler that supports C++11 features (i.e. GCC >= 4.7)

Building
========

1. Download and extract the latest source code tarball from [release](https://github.com/librehat/libQtShadowsocks/releases) (or `git clone` the latest code from `master` branch)
2. Run `qmake` to generate `Makefile`. By default, the `INSTALL_PREFIX` is `/usr`, and `BOTAN_VER` is `"1.10"`. If you want to install it to different location, or use a different version of Botan library, i.e. install to `/usr/local` and use Botan 1.11, then you need to run command `qmake INSTALL_PREFIX=/usr/local BOTAN_VER="1.1"`. If your distribution (i.e. Fedora) requires library installed into `/usr/lib64` on 64-bit system instead of `/usr/lib`, you have to add an extra argument `DEFINES+="LIB64"` to `qmake` command.
3. At last, compile and install it:
```
make
sudo make install
```

The above procedures will compile and install both `libQtShadowsocks` and `shadowsocks-libQtShadowsocks`. If you're a packager, you might need to split it into two packages depending on your distribution's guidelines.
