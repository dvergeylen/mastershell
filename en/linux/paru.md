---
layout: default
title: "paru"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="paru">
  <a href="/en/linux/paru.html">paru</a> <a href="#paru"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An AUR helper and pacman wrapper.
> More information: <https://github.com/Morganamilo/paru>.

#### Interactively search for and install a package:
```shell
paru {{package_name_or_seach_term}}
```
#### Synchronize and update all packages:
```shell
paru
```
#### Upgrade AUR packages:
```shell
paru -Sua
```
#### Get information about a package:
```shell
paru -Si {{package_name}}
```
#### Download `PKGBUILD` and other package source files from the AUR or ABS:
```shell
paru --getpkgbuild {{package_name}}
```
#### Display the `PKGBUILD` file of a package:
```shell
paru --getpkgbuild --print {{package_name}}
```
{% endraw %}