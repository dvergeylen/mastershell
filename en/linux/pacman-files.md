---
layout: default
title: "pacman --files"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---files">
  <a href="/en/linux/pacman-files.html">pacman --files</a> <a href="#pacman---files"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> See also `pkgfile`.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help:
```shell
pacman --files --help
```
#### Update the package database:
```shell
sudo pacman --files --refresh
```
#### Find the package that owns a specific file:
```shell
pacman --files {{filename}}
```
#### Find the package that owns a specific file, using a regular expression:
```shell
pacman --files --regex '{{regular_expression}}'
```
#### List only the package names:
```shell
pacman --files --quiet {{filename}}
```
#### List the files owned by a specific package:
```shell
pacman --files --list {{package_name}}
```
#### List only the absolute path to the files:
```shell
pacman --query --list --quiet {{package_name}}
```
{% endraw %}