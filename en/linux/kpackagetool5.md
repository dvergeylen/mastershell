---
layout: default
title: "kpackagetool5"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kpackagetool5">
  <a href="/en/linux/kpackagetool5.html">kpackagetool5</a> <a href="#kpackagetool5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KPackage Manager: Install, list, remove Plasma packages.
> More information: <https://techbase.kde.org/Development/Tutorials/Plasma5/QML2/GettingStarted#Kpackagetool5>.

#### List all known package types that can be installed:
```shell
kpackagetool5 --list-types
```
#### Install the package from a directory:
```shell
kpackagetool5 --type {{package_type}} --install {{path/to/directory}}
```
#### Update installed package from a directory:
```shell
kpackagetool5 --type {{package_type}} --upgrade {{path/to/directory}}
```
#### List installed plasmoids (--global for all users):
```shell
kpackagetool5 --type Plasma/Applet --list --global
```
#### Remove a plasmoid by name:
```shell
kpackagetool5 --type Plasma/Applet --remove "{{name}}"
```
{% endraw %}