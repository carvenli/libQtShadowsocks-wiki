##Microsoft Windows##

Need Windows Vista or later.

Prebuilt client `shadowsocks-libqss` are provided in [release](https://github.com/librehat/libQtShadowsocks/releases).

No prebuilt libraries are provided for Windows because of various compilers, Qt and Botan library versions.

##Fedora/Red Hat Enterprise Linux/CentOS##

Requirement: Fedora >= 21 or Red Hat Enterprise Linux >= 7

You can install this library and the client via [librehat/shadowsocks project in Copr](http://copr.fedoraproject.org/coprs/librehat/shadowsocks/).

##Debian/Ubuntu/Linux Mint/Deepin##

Requirement: Debian >= 7 or Ubuntu >= 14.04

For Ubuntu users, please use [PPA](https://code.launchpad.net/~hzwhuang/+archive/ubuntu/ss-qt5).

For Debian and other Debian-based distributions, build deb packages via commands below:

```bash
sudo apt-get install qt5-qmake qtbase5-dev libbotan1.10-dev #skip this part if you've already installed these packages
dpkg-buildpackage -uc -us -b
```

Then install `libqtshadowsocks` and `shadowsocks-libqtshadowsocks` deb packages using command `dpkg -i`.

##Other Operating Systems##
Check [Compiling](https://github.com/librehat/libQtShadowsocks/wiki/Compiling) page.