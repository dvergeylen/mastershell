---
layout: default
title: "apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt">
  <a href="/en/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for Debian based distributions.
> Recommended replacement for apt-get when used interactively in Ubuntu versions 16.04 and later.
> More information: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Update the list of available packages and versions (it's recommended to run this before other `apt` commands):
```shell
sudo apt update
```
#### Search for a given package:
```shell
apt search {{package}}
```
#### Show information for a package:
```shell
apt show {{package}}
```
#### Install a package, or update it to the latest available version:
```shell
sudo apt install {{package}}
```
#### Remove a package (using `purge` instead also removes its configuration files):
```shell
sudo apt remove {{package}}
```
#### Upgrade all installed packages to their newest available versions:
```shell
sudo apt upgrade
```
#### List all packages:
```shell
apt list
```
#### List installed packages:
```shell
apt list --installed
```
{% endraw %}