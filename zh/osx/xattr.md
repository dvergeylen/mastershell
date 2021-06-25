---
layout: default
title: "xattr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xattr">
  <a href="/zh/osx/xattr.html">xattr</a> <a href="#xattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于扩展文件系统属性的实用程序.

#### 列出 键：值 列表，显示指定文件的值扩展属性:
```shell
xattr -l {{文件名}}
```
#### 为给定文件写入属性:
```shell
xattr -w {{属性键名}} {{属性值}} {{文件名}}
```
#### 从给定文件中删除属性:
```shell
xattr -d {{com.apple.quarantine}} {{文件名}}
```
#### 从给定文件中删除所有扩展属性:
```shell
xattr -c {{文件名}}
```
#### 递归删除给定目录中文件的属性:
```shell
xattr -rd {{属性键名}} {{目录}}
```
{% endraw %}