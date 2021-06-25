---
layout: default
title: "ditto"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ditto">
  <a href="/zh/osx/ditto.html">ditto</a> <a href="#ditto"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制文件和目录.

#### 用源目录的内容覆盖目标目录的内容:
```shell
ditto {{源文件路径}} {{目标文件路径}}
```
#### 为复制的每个文件打印一行到终端窗口:
```shell
ditto -V {{源文件路径}} {{目标文件路径}}
```
#### 复制给定的文件或目录，同时保留原始文件权限:
```shell
ditto -rsrc {{源文件路径}} {{目标文件路径}}
```
{% endraw %}