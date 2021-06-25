---
layout: default
title: "port"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="port">
  <a href="/en/osx/port.html">port</a> <a href="#port"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package manager for macOS.

#### Search for a package:
```shell
port search {{search_term}}
```
#### Install a package:
```shell
sudo port install {{package_name}}
```
#### List installed packages:
```shell
port installed
```
#### Update port and fetch latest list of available packages:
```shell
sudo port selfupdate
```
#### Upgrade outdated packages:
```shell
sudo port upgrade outdated
```
#### Remove old versions of installed packages:
```shell
sudo port uninstall inactive
```
{% endraw %}