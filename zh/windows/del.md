---
layout: default
title: "del"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="del">
  <a href="/zh/windows/del.html">del</a> <a href="#del"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 删除一个或多个文件.

#### 删除一个或多个以空格分隔的文件:
```shell
del {{文件 文件 ..}}
```
#### 在删除每个文件之前提示确认:
```shell
del {{文件}} /p
```
#### 强制删除只读文件:
```shell
del {{文件}} /f
```
#### 递归删除所有子目录中的文件:
```shell
del {{文件}} /s
```
#### 在基于全局通配符删除文件时不提示确认:
```shell
del {{文件}} /q
```
#### 显示帮助和所有的属性列表:
```shell
del /?
```
#### 根据指定的属性删除文件:
```shell
del {{文件}} /a {{属性}}
```
{% endraw %}