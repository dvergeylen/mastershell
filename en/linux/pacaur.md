---
layout: default
title: "pacaur"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacaur">
  <a href="/en/linux/pacaur.html">pacaur</a> <a href="#pacaur"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility for Arch Linux to build and install packages from the Arch User Repository.

#### Synchronize and update all packages (includes AUR):
```shell
pacaur -Syu
```
#### Synchronize and update only AUR packages:
```shell
pacaur -Syua
```
#### Install a new package (includes AUR):
```shell
pacaur -S {{package_name}}
```
#### Remove a package and its dependencies (includes AUR packages):
```shell
pacaur -Rs {{package_name}}
```
#### Search the package database for a keyword (includes AUR):
```shell
pacaur -Ss {{keyword}}
```
#### List all currently installed packages (includes AUR packages):
```shell
pacaur -Qs
```
{% endraw %}