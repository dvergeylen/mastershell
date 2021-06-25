---
layout: default
title: "apt-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-cache">
  <a href="/en/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian and Ubuntu package query tool.
> More information: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Search for a package in your current sources:
```shell
apt-cache search {{query}}
```
#### Show information about a package:
```shell
apt-cache show {{package}}
```
#### Show whether a package is installed and up to date:
```shell
apt-cache policy {{package}}
```
#### Show dependencies for a package:
```shell
apt-cache depends {{package}}
```
#### Show packages that depend on a particular package:
```shell
apt-cache rdepends {{package}}
```
{% endraw %}