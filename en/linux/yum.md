---
layout: default
title: "yum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yum">
  <a href="/en/linux/yum.html">yum</a> <a href="#yum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for RHEL, Fedora, and CentOS (for older versions).
> More information: <https://man7.org/linux/man-pages/man8/yum.8.html>.

#### Install a new package:
```shell
yum install {{package}}
```
#### Install a new package and assume yes to all questions (also works with update, great for automated updates):
```shell
yum -y install {{package}}
```
#### Find the package that provides a particular command:
```shell
yum provides {{command}}
```
#### Remove a package:
```shell
yum remove {{package}}
```
#### Display available updates for installed packages:
```shell
yum check-update
```
#### Upgrade installed packages to newest available versions:
```shell
yum upgrade
```
{% endraw %}