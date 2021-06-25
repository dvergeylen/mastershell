---
layout: default
title: "debuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="debuild">
  <a href="/en/linux/debuild.html">debuild</a> <a href="#debuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to build a Debian package from source.
> More information: <https://manpages.debian.org/debuild>.

#### Build the package in the current directory:
```shell
debuild
```
#### Build a binary package only:
```shell
debuild -b
```
#### Do not run lintian after building the package:
```shell
debuild --no-lintian
```
{% endraw %}