---
layout: default
title: "yaourt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yaourt">
  <a href="/en/linux/yaourt.html">yaourt</a> <a href="#yaourt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux utility for building packages from the Arch User Repository.

#### Synchronize and update all packages (including AUR):
```shell
yaourt -Syua
```
#### Install a new package (includes AUR):
```shell
yaourt -S {{package_name}}
```
#### Remove a package and its dependencies (includes AUR packages):
```shell
yaourt -Rs {{package_name}}
```
#### Search the package database for a keyword (including AUR):
```shell
yaourt -Ss {{package_name}}
```
#### List installed packages, versions, and repositories (AUR packages will be listed under the repository name 'local'):
```shell
yaourt -Q
```
{% endraw %}