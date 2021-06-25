---
layout: default
title: "trizen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="trizen">
  <a href="/en/linux/trizen.html">trizen</a> <a href="#trizen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux utility for building packages from the Arch User Repository (AUR).

#### Synchronize and update all AUR packages:
```shell
trizen -Syua
```
#### Install a new package:
```shell
trizen -S {{package}}
```
#### Remove a package and its dependencies:
```shell
trizen -Rs {{package}}
```
#### Search the package database for a keyword:
```shell
trizen -Ss {{keyword}}
```
#### Show information about a package:
```shell
trizen -Si {{package}}
```
#### List installed packages and versions:
```shell
trizen -Qe
```
{% endraw %}