---
layout: default
title: "pkginfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pkginfo">
  <a href="/en/linux/pkginfo.html">pkginfo</a> <a href="#pkginfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the package database on a CRUX system.

#### List installed packages and their versions:
```shell
pkginfo -i
```
#### List files owned by a package:
```shell
pkginfo -l {{package_name}}
```
#### List the owner(s) of files matching a pattern:
```shell
pkginfo -o {{pattern}}
```
#### Print the footprint of a file:
```shell
pkginfo -f {{file}}
```
{% endraw %}