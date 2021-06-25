---
layout: default
title: "mac2unix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mac2unix">
  <a href="/zh/linux/mac2unix.html">mac2unix</a> <a href="#mac2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 macOS 样式的行尾更改为 Unix 样式.
> 用 CR 替换 LF.

#### 更改文件的行尾:
```shell
mac2unix {{文件名}}
```
#### 使用 Unix 样式的行尾创建副本:
```shell
mac2unix -n {{文件名}} {{新文件名}}
```
{% endraw %}