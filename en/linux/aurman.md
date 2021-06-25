---
layout: default
title: "aurman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aurman">
  <a href="/en/linux/aurman.html">aurman</a> <a href="#aurman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An Arch Linux utility to build and install packages from the Arch User Repository.
> See also `pacman`.
> More information: <https://github.com/polygamma/aurman>.

#### Synchronize and update all packages:
```shell
aurman --sync --refresh --sysupgrade
```
#### Synchronize and update all packages without show changes of `PKGBUILD` files:
```shell
aurman --sync --refresh --sysupgrade --noedit
```
#### Install a new package:
```shell
aurman --sync {{package_name}}
```
#### Install a new package without show changes of `PKGBUILD` files:
```shell
aurman --sync --noedit {{package_name}}
```
#### Install a new package without prompting:
```shell
aurman --sync --noedit --noconfirm {{package_name}}
```
#### Search the package database for a keyword from the official repositories and AUR:
```shell
aurman --sync --search {{keyword}}
```
#### Remove a package and its dependencies:
```shell
aurman --remove --recursive --nosave {{package_name}}
```
#### Clear the package cache (use two `--clean` flags to clean all packages):
```shell
aurman --sync --clean
```
{% endraw %}