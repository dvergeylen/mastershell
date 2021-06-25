---
layout: default
title: "stat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stat">
  <a href="/en/common/stat.html">stat</a> <a href="#stat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display file and filesystem information.

#### Show file properties such as size, permissions, creation and access dates among others:
```shell
stat {{file}}
```
#### Same as above but in a more concise way:
```shell
stat -t {{file}}
```
#### Show filesystem information:
```shell
stat -f {{file}}
```
#### Show only octal file permissions:
```shell
stat -c "%a %n" {{file}}
```
#### Show owner and group of the file:
```shell
stat -c "%U %G" {{file}}
```
#### Show the size of the file in bytes:
```shell
stat -c "%s %n" {{file}}
```
{% endraw %}