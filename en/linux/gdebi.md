---
layout: default
title: "gdebi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gdebi">
  <a href="/en/linux/gdebi.html">gdebi</a> <a href="#gdebi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple tool to install `.deb` files.
> More information: <https://www.commandlinux.com/man-page/man1/gdebi.1.html>.

#### Install local `.deb` packages resolving and installing its dependencies:
```shell
gdebi {{path/to/package.deb}}
```
#### Display the program version:
```shell
gdebi --version
```
#### Do not show progress information:
```shell
gdebi {{path/to/package.deb}} --quiet
```
#### Set an APT configuration option:
```shell
gdebi {{path/to/package.deb}} --option={{APT_OPTS}}
```
#### Use alternative root dir:
```shell
gdebi {{path/to/package.deb}} --root={{path/to/root_dir}}
```
{% endraw %}