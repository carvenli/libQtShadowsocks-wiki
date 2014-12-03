The namespace of `libQtShadowsocks` is shortened as `QSS`, which stands for Qt, Shadow, Socks respectively.

You can subclass `BaseController` to write your own controller classes. While the recommended way to utilise this library is to use `LocalController` and `ServerController`(TODO) directly.

The project `sslocal-libqss` in the directory `client` is used as a demonstration to show you how to use `LocalController` class.

Do bear in mind that all dependencies of `libQtShadowsocks` will be passed to your project as well. That is, including `QtCore`, `QtNetwork`, `QtConcurrent` and `QCA`.