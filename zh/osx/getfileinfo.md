---
layout: default
title: "GetFileInfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getfileinfo">
  <a href="/zh/osx/getfileinfo.html">GetFileInfo</a> <a href="#getfileinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 获取有关 HFS+ 目录中文件的信息.

#### 显示有关给定文件的信息:
```shell
GetFileInfo {{路径/文件名}}
```
#### 显示给定文件的创建日期和时间:
```shell
GetFileInfo -d {{路径/文件名}}
```
#### 显示给定文件的上次修改日期和时间:
```shell
GetFileInfo -m {{路径/文件名}}
```
#### 显示给定文件的创建者:
```shell
GetFileInfo -c {{路径/文件名}}
```
{% endraw %}