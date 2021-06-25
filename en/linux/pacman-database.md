---
layout: default
title: "pacman --database"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---database">
  <a href="/en/linux/pacman-database.html">pacman --database</a> <a href="#pacman---database"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Operate on the Arch Linux package database.
> Modify certain attributes of the installed packages.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help:
```shell
pacman --database --help
```
#### Mark a package as implicitly installed:
```shell
sudo pacman --database --asdeps {{package_name}}
```
#### Mark a package as explicitly installed:
```shell
sudo pacman --database --asexplicit {{package_name}}
```
#### Check that all the package dependencies are installed:
```shell
pacman --database --check
```
#### Check the repositories to ensure all specified dependencies are available:
```shell
pacman --database --check --check
```
#### Display only error messages:
```shell
pacman --database --check --quiet
```
{% endraw %}