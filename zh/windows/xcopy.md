---
layout: default
title: "xcopy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcopy">
  <a href="/zh/windows/xcopy.html">xcopy</a> <a href="#xcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制文件和目录树.

#### 复制文件到指定的路径:
```shell
xcopy {{被复制的目录路径}} {{目标路径}}
```
#### 列出在复制前将要被复制的文件:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /p
```
#### 仅复制目录结构，不包括文件:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /t
```
#### 复制时包含空目录:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /e
```
#### 复制文件时保留 ACL 信息:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /o
```
#### 网络连接丢失时允许恢复:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /z
```
#### 当文件存在于目标路径中时禁用提示
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /y
```
#### 显示详细的使用帮助:
```shell
xcopy /?
```
{% endraw %}