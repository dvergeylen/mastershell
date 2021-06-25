---
layout: default
title: "dir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dir">
  <a href="/zh/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 列出目录的内容.

#### 显示当前目录的内容:
```shell
dir
```
#### 显示指定目录的内容:
```shell
dir {{目录的路径}}
```
#### 显示当前目录的内容，包括隐藏的文件:
```shell
dir /A
```
#### 显示指定目录的内容，包括隐藏的文件:
```shell
dir {{目录的路径}} /A
```
{% endraw %}