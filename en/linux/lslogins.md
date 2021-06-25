---
layout: default
title: "lslogins"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lslogins">
  <a href="/en/linux/lslogins.html">lslogins</a> <a href="#lslogins"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about users on a Linux system.
> More information: <https://man7.org/linux/man-pages/man1/lslogins.1.html>.

#### Display users in the system:
```shell
lslogins
```
#### Display users belonging to a specific group:
```shell
lslogins --groups={{groups}}
```
#### Display user accounts:
```shell
lslogins --user-accs
```
#### Display last logins:
```shell
lslogins --last
```
#### Display system accounts:
```shell
lslogins --system-accs
```
#### Display supplementary groups:
```shell
lslogins --supp-groups
```
{% endraw %}