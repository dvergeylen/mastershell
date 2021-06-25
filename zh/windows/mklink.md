---
layout: default
title: "mklink"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mklink">
  <a href="/zh/windows/mklink.html">mklink</a> <a href="#mklink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建符号链接.

#### 创建指向文件的符号链接:
```shell
mklink {{链接文件的路径}} {{源文件路径}}
```
#### 创建指向目录的符号链接:
```shell
mklink /d {{链接文件的路径}} {{源目录路径}}
```
#### 创建指向文件的硬链接:
```shell
mklink /h {{链接文件的路径}} {{源目录路径}}
```
#### 创建目录链接:
```shell
mklink /j {{链接文件的路径}} {{源目录路径}}
```
{% endraw %}