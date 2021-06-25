---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/zh/windows/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 以目录树的形式显示指定目录的所有文件夹和文件.

#### 显示当前目录的目录树:
```shell
tree
```
#### 显示指定目录的目录树:
```shell
tree {{目录的路径}}
```
#### 显示目录中文件的目录树:
```shell
tree {{目录的路径}} /f
```
#### 使用 ASCII 字符而不是扩展字符显示目录树:
```shell
tree {{目录的路径}} /a
```
{% endraw %}