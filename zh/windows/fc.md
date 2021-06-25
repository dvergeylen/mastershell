---
layout: default
title: "fc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fc">
  <a href="/zh/windows/fc.html">fc</a> <a href="#fc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 比较两个文件或文件集之间的差异.
> 使用通配符 (*) 来比较文件集.

#### 比较两个指定的文件:
```shell
fc {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 比较时不区分大小写:
```shell
fc /c {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 将文件作为 Unicode 文本来进行比较:
```shell
fc /u {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 将文件作为 ASCII 文本来进行比较:
```shell
fc /l {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 将文件作为二进制来比较:
```shell
fc /b {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 禁用制表符到空格的扩展:
```shell
fc /t {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 压缩空格（制表符和空格）进行比较:
```shell
fc /w {{文件 1 的路径}} {{文件 2 的路径}}
```
{% endraw %}