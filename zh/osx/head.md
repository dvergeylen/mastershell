---
layout: default
title: "head"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="head">
  <a href="/zh/osx/head.html">head</a> <a href="#head"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 输出文件的开头部分.

#### 输出文件的前几行:
```shell
head -n {{行数}} {{文件名}}
```
#### 输出文件的前几个字节:
```shell
head -c {{字节数}} {{文件名}}
```
{% endraw %}