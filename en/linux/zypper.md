---
layout: default
title: "zypper"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zypper">
  <a href="/en/linux/zypper.html">zypper</a> <a href="#zypper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SUSE & openSUSE package management utility.

#### Synchronize list of packages and versions available:
```shell
zypper refresh
```
#### Install a new package:
```shell
zypper install {{package}}
```
#### Remove a package:
```shell
zypper remove {{package}}
```
#### Upgrade installed packages to newest available versions:
```shell
zypper update
```
#### Search package via keyword:
```shell
zypper search {{keyword}}
```
{% endraw %}