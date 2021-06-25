---
layout: default
title: "mkfile"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfile">
  <a href="/zh/osx/mkfile.html">mkfile</a> <a href="#mkfile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建一个或多个任意大小的空文件.

#### 创建一个 15 千字节的空文件:
```shell
mkfile -n {{15k}} {{文件名}}
```
#### 创建给定大小和单位的文件 (bytes, KB, MB, GB):
```shell
mkfile -n {{大小}}{{b|k|m|g}} {{文件名}}
```
#### 创建两个 4 兆字节的文件:
```shell
mkfile -n {{4m}} {{文件名 1}} {{文件名 2}}
```
{% endraw %}