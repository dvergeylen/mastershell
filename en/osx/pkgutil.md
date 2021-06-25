---
layout: default
title: "pkgutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pkgutil">
  <a href="/en/osx/pkgutil.html">pkgutil</a> <a href="#pkgutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query and manipulate Mac OS X Installer packages and receipts.

#### List package IDs for all installed packages:
```shell
pkgutil --pkgs
```
#### Verify cryptographic signatures of a package file:
```shell
pkgutil --check-signature {{path/to/filename.pkg}}
```
#### List all the files for an installed package given its ID:
```shell
pkgutil --files {{com.microsoft.Word}}
```
#### Extract the contents of a package file into a directory:
```shell
pkgutil --expand-full {{path/to/filename.pkg}} {{path/to/directory}}
```
{% endraw %}