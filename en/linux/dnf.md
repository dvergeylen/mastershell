---
layout: default
title: "dnf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dnf">
  <a href="/en/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for RHEL, Fedora, and CentOS (replaces yum).
> More information: <https://dnf.readthedocs.io/>.

#### Upgrade installed packages to the newest available versions:
```shell
sudo dnf upgrade
```
#### Search packages via keywords:
```shell
dnf search {{keywords}}
```
#### Display details about a package:
```shell
dnf info {{package}}
```
#### Install a new package:
```shell
sudo dnf install {{package}}
```
#### Install a new package and assume yes to all questions:
```shell
sudo dnf -y install {{package}}
```
#### Remove a package:
```shell
sudo dnf remove {{package}}
```
#### List installed packages:
```shell
dnf list --installed
```
#### Find which packages provide a given file:
```shell
dnf provides {{file}}
```
{% endraw %}