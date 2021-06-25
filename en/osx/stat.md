---
layout: default
title: "stat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stat">
  <a href="/en/osx/stat.html">stat</a> <a href="#stat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display file status.

#### Show file properties such as size, permissions, creation and access dates among others:
```shell
stat {{file}}
```
#### Same as above but verbose (more similar to linux's `stat`):
```shell
stat -x {{file}}
```
#### Show only octal file permissions:
```shell
stat -f %Mp%Lp {{file}}
```
#### Show owner and group of the file:
```shell
stat -f "%Su %Sg" {{file}}
```
#### Show the size of the file in bytes:
```shell
stat -f "%z %N" {{file}}
```
{% endraw %}