---
layout: default
title: "prt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="prt-get">
  <a href="/en/linux/prt-get.html">prt-get</a> <a href="#prt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The CRUX package manager.

#### Install a package:
```shell
prt-get install {{package_name}}
```
#### Install a package with dependency handling:
```shell
prt-get depinst {{package_name}}
```
#### Update a package manually:
```shell
prt-get upgrade {{package_name}}
```
#### Remove a package:
```shell
prt-get remove {{package_name}}
```
#### Upgrade the system from the local ports tree:
```shell
prt-get sysup
```
#### Search the ports tree:
```shell
prt-get search {{package_name}}
```
#### Search for a file in a package:
```shell
prt-get fsearch {{file}}
```
{% endraw %}