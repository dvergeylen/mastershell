---
layout: default
title: "unix2mac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unix2mac">
  <a href="/zh/linux/unix2mac.html">unix2mac</a> <a href="#unix2mac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 Unix 样式的行尾更改为 macOS 样式.
> 用 LF 替换 CR.

#### 更改文件的行尾:
```shell
unix2mac {{文件名}}
```
#### 使用 macOS 样式的行尾创建副本:
```shell
unix2mac -n {{文件名}} {{新文件名}}
```
{% endraw %}