---
layout: default
title: "opkg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="opkg">
  <a href="/en/linux/opkg.html">opkg</a> <a href="#opkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A lightweight package manager used to install OpenWrt packages.

#### Install a package:
```shell
opkg install {{package}}
```
#### Remove a package:
```shell
opkg remove {{package}}
```
#### Update the list of available packages:
```shell
opkg update
```
#### Upgrade all the installed packages:
```shell
opkg upgrade
```
#### Upgrade one or more specific package(s):
```shell
opkg upgrade {{package(s)}}
```
#### Display information for a specific package:
```shell
opkg info {{package}}
```
#### List all the available packages:
```shell
opkg list
```
{% endraw %}