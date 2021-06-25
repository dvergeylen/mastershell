---
layout: default
title: "dos2unix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dos2unix">
  <a href="/zh/linux/dos2unix.html">dos2unix</a> <a href="#dos2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 DOS 样式的行尾更改为 Unix 样式.
> 用 CR 替换 CRLF.

#### 更改文件的行尾:
```shell
dos2unix {{文件名}}
```
#### 使用 Unix 样式的行尾创建副本:
```shell
dos2unix -n {{文件名}} {{文件名}}
```
{% endraw %}