---
layout: default
title: "pacman --upgrade"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---upgrade">
  <a href="/en/linux/pacman-upgrade.html">pacman --upgrade</a> <a href="#pacman---upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help:
```shell
pacman --upgrade --help
```
#### Install one or more packages from files:
```shell
sudo pacman --upgrade {{path/to/package1.pkg.tar.zst}} {{path/to/package2.pkg.tar.zst}}
```
#### Install a package without prompting:
```shell
sudo pacman --upgrade --noconfirm {{path/to/package.pkg.tar.zst}}
```
#### Overwrite conflicting files during a package installation:
```shell
sudo pacman --upgrade --overwrite {{path/to/file}} {{path/to/package.pkg.tar.zst}}
```
#### Install a package, skipping the dependency version checks:
```shell
sudo pacman --upgrade --nodeps {{path/to/package.pkg.tar.zst}}
```
#### List packages that would be affected (does not install any packages):
```shell
pacman --query --print {{path/to/package.pkg.tar.zst}}
```
{% endraw %}