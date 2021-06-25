---
layout: default
title: "pamac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pamac">
  <a href="/en/linux/pamac.html">pamac</a> <a href="#pamac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line utility for the GUI package manager pamac.
> If you can't see the AUR packages, enable it in `/etc/pamac.conf` or in the GUI.
> More information: <https://wiki.manjaro.org/index.php/Pamac>.

#### Install a new package:
```shell
pamac install {{package_name}}
```
#### Remove a package and its no longer required dependencies (orphans):
```shell
pamac remove --orphans {{package_name}}
```
#### Search the package database for a package:
```shell
pamac search {{package_name}}
```
#### List installed packages:
```shell
pamac list --installed
```
#### Check for package updates:
```shell
pamac checkupdates
```
#### Upgrade all packages:
```shell
pamac upgrade
```
{% endraw %}