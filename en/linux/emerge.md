---
layout: default
title: "emerge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emerge">
  <a href="/en/linux/emerge.html">emerge</a> <a href="#emerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gentoo Linux package manager utility.

#### Synchronize all packages:
```shell
emerge --sync
```
#### Update all packages, including dependencies:
```shell
emerge -uDNav @world
```
#### Resume a failed updated, skipping the failing package:
```shell
emerge --resume --skipfirst
```
#### Install a new package, with confirmation:
```shell
emerge -av {{package_name}}
```
#### Remove a package, with confirmation:
```shell
emerge -Cav {{package_name}}
```
#### Remove orphaned packages (that were installed only as dependencies):
```shell
emerge -avc
```
#### Search the package database for a keyword:
```shell
emerge -S {{keyword}}
```
{% endraw %}