---
layout: default
title: "xbps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xbps">
  <a href="/en/linux/xbps.html">xbps</a> <a href="#xbps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The X Binary Package System (or xbps) is the binary package system used by Void Linux.
> More information: <https://github.com/void-linux/xbps>.

#### Install packages and synchronize them with the remote repository:
```shell
xbps-install --synchronize {{package_name1}} {{package_name2}}
```
#### Search for a package in the remote repository:
```shell
xbps-query --repository -s {{package_name}}
```
#### Remove a package, leaving all of its dependencies installed:
```shell
xbps-remove {{package_name}}
```
#### Remove a package and all of its dependencies recursively that are not required by other packages:
```shell
xbps-remove --recursive {{package_name}}
```
#### Synchronize your repository databases and update your system and dependencies:
```shell
xbps-install --synchronize -u
```
#### Remove packages that were installed as dependencies and aren't currently needed:
```shell
xbps-remove --remove-orphans
```
#### Remove obsolete packages from the cache:
```shell
xbps-remove --clean-cache
```
{% endraw %}