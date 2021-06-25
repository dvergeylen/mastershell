---
layout: default
title: "pacman --deptest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---deptest">
  <a href="/en/linux/pacman-deptest.html">pacman --deptest</a> <a href="#pacman---deptest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check each dependency specified and return a list of dependencies that are not currently satisfied on the system.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Print the package names of the dependencies that aren't installed:
```shell
pacman --deptest {{package_name1}} {{package_name2}}
```
#### Check if the installed package satisfies the given minimum version:
```shell
pacman --deptest "{{bash>=5}}"
```
#### Check if a later version of a package is installed:
```shell
pacman --deptest "{{bash>5}}"
```
#### Display help:
```shell
pacman --deptest --help
```
{% endraw %}