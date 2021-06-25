---
layout: default
title: "apt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-get">
  <a href="/en/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian and Ubuntu package management utility.
> Search for packages using `apt-cache`.
> More information: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Update the list of available packages and versions (it's recommended to run this before other `apt-get` commands):
```shell
apt-get update
```
#### Install a package, or update it to the latest available version:
```shell
apt-get install {{package}}
```
#### Remove a package:
```shell
apt-get remove {{package}}
```
#### Remove a package and its configuration files:
```shell
apt-get purge {{package}}
```
#### Upgrade all installed packages to their newest available versions:
```shell
apt-get upgrade
```
#### Clean the local repository - removing package files (`.deb`) from interrupted downloads that can no longer be downloaded:
```shell
apt-get autoclean
```
#### Remove all packages that are no longer needed:
```shell
apt-get autoremove
```
#### Upgrade installed packages (like `upgrade`), but remove obsolete packages and install additional packages to meet new dependencies:
```shell
apt-get dist-upgrade
```
{% endraw %}