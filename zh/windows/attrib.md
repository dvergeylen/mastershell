---
layout: default
title: "attrib"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="attrib">
  <a href="/zh/windows/attrib.html">attrib</a> <a href="#attrib"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或修改文件和目录的属性.

#### 显示当前目录下所有文件的属性:
```shell
attrib
```
#### 显示当前目录和其子目录下所有文件的属性:
```shell
attrib /S
```
#### 显示当前目录和其子目录下所有文件和目录的属性:
```shell
attrib /S /D
```
#### 为一个文件增加只读属性:
```shell
attrib +R {{document.txt}}
```
#### 删除一个文件的系统和隐藏属性:
```shell
attrib -S -H {{document.txt}}
```
#### 为一个目录增加隐藏属性:
```shell
attrib +H {{目录的路径}}
```
{% endraw %}