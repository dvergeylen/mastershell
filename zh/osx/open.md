---
layout: default
title: "open"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="open">
  <a href="/zh/osx/open.html">open</a> <a href="#open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打开文件、目录和应用程序.

#### 使用系统关联的应用程序打开文件:
```shell
open {{filename.extension}}
```
#### 运行图形化的 macOS 应用程序:
```shell
open -a {{应用程序名}}
```
#### 运行指定 包名 的图形化 macOS 应用程序（请参阅`OSascript`命令，查询如何获取应用程序的 包名）:
```shell
open -b {{com.domain.application 应用程序包名}}
```
#### 在"访达 (finder)"中打开当前文件夹:
```shell
open .
```
#### 打开"访达 (finder)", 并且给出指定文件:
```shell
open -R {{文件路径}}
```
#### 使用系统默认应用程序，打开当前目录中所有给定扩展名的文件:
```shell
open {{*.extension}}
```
{% endraw %}