---
layout: default
title: "pacman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman">
  <a href="/en/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Synchronize and update all packages:
```shell
pacman --sync --refresh --sysupgrade
```
#### Install a new package:
```shell
pacman --sync {{package_name}}
```
#### Remove a package and its dependencies:
```shell
pacman --remove --recursive {{package_name}}
```
#### Search the package database for a regular expression or keyword:
```shell
pacman --sync --search "{{search_pattern}}"
```
#### List installed packages and versions:
```shell
pacman --query
```
#### List only the explicitly installed packages and versions:
```shell
pacman --query --explicit
```
#### List orphan packages (installed as dependencies but not actually required by any package):
```shell
pacman --query --unrequired --deps --quiet
```
#### Empty the entire pacman cache:
```shell
pacman --sync --clean --clean
```
{% endraw %}