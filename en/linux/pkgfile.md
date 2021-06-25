---
layout: default
title: "pkgfile"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pkgfile">
  <a href="/en/linux/pkgfile.html">pkgfile</a> <a href="#pkgfile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for searching files from packages in the official repositories on arch-based systems.
> See also `pacman files`, describing the usage of `pacman --files`.
> More information: <https://man.archlinux.org/man/extra/pkgfile/pkgfile.1>.

#### Synchronize the pkgfile database:
```shell
sudo pkgfile --update
```
#### Search for a package that owns a specific file:
```shell
pkgfile {{filename}}
```
#### List all files provided by a package:
```shell
pkgfile --list {{package_name}}
```
#### List only files provided by a package located within the `bin` or `sbin` directory:
```shell
pkgfile --list --binaries {{package_name}}
```
#### Search for a package that owns a specific file using case insensitive matching:
```shell
pkgfile --ignorecase {{filename}}
```
#### Search for a package that owns a specific file in the `bin` or `sbin` directory:
```shell
pkgfile --binaries {{filename}}
```
#### Search for a package that owns a specific file, displaying the package version:
```shell
pkgfile --verbose {{filename}}
```
#### Search for a package that owns a specific file in a specific repository:
```shell
pkgfile --repo {{repository_name}} {{filename}}
```
{% endraw %}