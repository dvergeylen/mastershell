---
layout: default
title: "slapt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="slapt-get">
  <a href="/en/linux/slapt-get.html">slapt-get</a> <a href="#slapt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An apt like system for Slackware package management.
> Package sources need to be configured in the slapt-getrc file.

#### Update the list of available packages and versions:
```shell
slapt-get --update
```
#### Install a package, or update it to the latest available version:
```shell
slapt-get --install {{package_name}}
```
#### Remove a package:
```shell
slapt-get --remove {{package_name}}
```
#### Upgrade all installed packages to their latest available versions:
```shell
slapt-get --upgrade
```
#### Locate packages of interest by the package name, disk set, or version:
```shell
slapt-get --search {{package_name}}
```
#### Show information about a package:
```shell
slapt-get --show {{package_name}}
```
{% endraw %}