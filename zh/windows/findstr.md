---
layout: default
title: "findstr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="findstr">
  <a href="/zh/windows/findstr.html">findstr</a> <a href="#findstr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在一个或多个文件中查找指定的文本.

#### 在所有文件中查找以空格分隔的字符串:
```shell
findstr "{{查询语句 查询语句 ..}}" *
```
#### 以递归方式在所有文件中查找以空格分隔的字符串:
```shell
findstr /s "{{查询语句 查询语句 ..}}" *
```
#### 查找时不区分大小写:
```shell
findstr /i "{{查询语句}}" *"
```
#### 使用正则表达式搜索:
```shell
findstr /r "{{正则表达式}}" *
```
#### 在所有文本文件中查找文字字符串（包含空格）:
```shell
findstr /c:"{{查询语句}}" *.txt
```
#### 只查找完全匹配的行:
```shell
findstr /x "{{查询语句}}" *
```
#### 显示匹配的行的行数:
```shell
findstr /n "{{查询语句}}" *
```
#### 只显示匹配的文件名:
```shell
findstr /m "{{查询语句}}" *
```
{% endraw %}