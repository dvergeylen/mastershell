---
layout: default
title: "yay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yay">
  <a href="/en/linux/yay.html">yay</a> <a href="#yay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yet Another Yogurt: A utility for Arch Linux to build and install packages from the Arch User Repository.
> Also see `pacman`.
> More information: <https://github.com/Jguer/yay>.

#### Interactively search and install packages from the repos and AUR:
```shell
yay {{package_name|search_term}}
```
#### Synchronize and update all packages from the repos and AUR:
```shell
yay
```
#### Synchronize and update only AUR packages:
```shell
yay -Sua
```
#### Install a new package from the repos and AUR:
```shell
yay -S {{package_name}}
```
#### Remove an installed package and both its dependencies and configuration files:
```shell
yay -Rns {{package_name}}
```
#### Search the package database for a keyword from the repos and AUR:
```shell
yay -Ss {{keyword}}
```
#### Show statistics for installed packages and system health:
```shell
yay -Ps
```
{% endraw %}