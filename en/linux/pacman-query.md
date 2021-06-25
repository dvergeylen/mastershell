---
layout: default
title: "pacman --query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---query">
  <a href="/en/linux/pacman-query.html">pacman --query</a> <a href="#pacman---query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### List installed packages and versions:
```shell
pacman --query
```
#### List only packages and versions that were explicitly installed:
```shell
pacman --query --explicit
```
#### Find which package owns a file:
```shell
pacman --query --owns {{filename}}
```
#### Display information about an installed package:
```shell
pacman --query --info {{package_name}}
```
#### List files owned by a package:
```shell
pacman --query --list {{package_name}}
```
#### List orphan packages (installed as dependencies but not required by any package):
```shell
pacman --query --unrequired --deps --quiet
```
#### List installed packages not found in the repositories:
```shell
pacman --query --foreign
```
#### List outdated packages:
```shell
pacman --query --upgrades
```
{% endraw %}