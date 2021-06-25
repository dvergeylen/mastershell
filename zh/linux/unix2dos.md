---
layout: default
title: "unix2dos"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unix2dos">
  <a href="/zh/linux/unix2dos.html">unix2dos</a> <a href="#unix2dos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 Unix 样式的行尾更改为 DOS 样式.
> 用 CRLF 替换 CR.

#### 更改文件的行尾:
```shell
unix2dos {{文件名}}
```
#### 使用 DOS 样式的行尾创建副本:
```shell
unix2dos -n {{文件名}} {{新文件名}}
```
{% endraw %}