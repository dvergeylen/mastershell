---
layout: default
title: "sysctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sysctl">
  <a href="/en/linux/sysctl.html">sysctl</a> <a href="#sysctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List and change kernel runtime variables.

#### Show all available variables and their values:
```shell
sysctl -a
```
#### Set a changeable kernel state variable:
```shell
sysctl -w {{section.tunable}}={{value}}
```
#### Get currently open file handlers:
```shell
sysctl fs.file-nr
```
#### Get limit for simultaneous open files:
```shell
sysctl fs.file-max
```
#### Apply changes from `/etc/sysctl.conf`:
```shell
sysctl -p
```
{% endraw %}