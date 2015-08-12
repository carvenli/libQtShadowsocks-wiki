The namespace of `libQtShadowsocks` is shortened as `QSS`, which stands for **Q**t**S**hadow**S**ocks respectively.

You can subclass `Controller` to write your own controller classes. While the recommended way to utilise this library is to use `Controller` directly. `Controller` can be used either as `local` or `server` controller.

The sub-project `shadowsocks-libqss` is used as a demonstration to show you how to use `libQtShadowsocks`.

Do bear in mind that all dependencies of `libQtShadowsocks` will be passed to your project as well. That is, including `QtCore`, `QtNetwork`, and `Botan`.