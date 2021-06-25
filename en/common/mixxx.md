---
layout: default
title: "mixxx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mixxx">
  <a href="/en/common/mixxx.html">mixxx</a> <a href="#mixxx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Free and open source cross-platform DJ software.
> More information: <https://mixxx.org/manual/latest/chapters/appendix.html#command-line-options>.

#### Start the Mixxx GUI in fullscreen:
```shell
mixxx --fullScreen
```
#### Start in safe developer mode to debug a crash:
```shell
mixxx --developer --safeMode
```
#### Debug a malfunction:
```shell
mixxx --debugAssertBreak --developer --loglevel trace
```
#### Start mixxx using the specified settings file:
```shell
mixxx --resourcePath {{mixxx/res/controllers}} --settingsPath {{path/to/settings-file}}
```
#### Debug a custom controller mapping:
```shell
mixxx --controllerDebug --resourcePath {{path/to/mapping-directory}}
```
#### Show command-line help:
```shell
mixxx --help
```
{% endraw %}