---
layout: default
title: "pkgmk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pkgmk">
  <a href="/en/linux/pkgmk.html">pkgmk</a> <a href="#pkgmk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Make a binary package for use with pkgadd on CRUX.

#### Make and download a package:
```shell
pkgmk -d
```
#### Install the package after making it:
```shell
pkgmk -d -i
```
#### Upgrade the package after making it:
```shell
pkgmk -d -u
```
#### Ignore the footprint when making a package:
```shell
pkgmk -d -if
```
#### Ignore the MD5 sum when making a package:
```shell
pkgmk -d -im
```
#### Update the package's footprint:
```shell
pkgmk -uf
```
{% endraw %}