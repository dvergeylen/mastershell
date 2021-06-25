---
layout: default
title: "find"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="find">
  <a href="/zh/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在一个或多个文件里查找指定字符串.

#### 查找包含指定字符串的行:
```shell
find {{字符串}} {{文件或目录的路径}}
```
#### 查找不包含指定字符串的行:
```shell
find {{字符串}} {{文件或目录的路径}} /v
```
#### 显示包含指定字符串的行的总数:
```shell
find {{字符串}} {{文件或目录的路径}} /c
```
#### 显示匹配的行的行数:
```shell
find {{字符串}} {{文件或目录的路径}} /n
```
{% endraw %}