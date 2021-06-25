---
layout: default
title: "du"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="du">
  <a href="/zh/osx/du.html">du</a> <a href="#du"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 磁盘使用率：估计和汇总文件和目录空间使用率.

#### 以给定单位（kb/mb/gb）列出目录和所有子目录的大小:
```shell
du -{{k|m|g}} {{目标文件夹}}
```
#### 以可读形式列出目录和任何子目录的大小（即自动为转换为选择的适当单位 kb|mb|gb）:
```shell
du -h {{目标文件夹}}
```
#### 以可读单位显示目录大小:
```shell
du -sh {{目标文件夹}}
```
#### 列出目录以及其中所有文件和目录的可读大小:
```shell
du -ah {{目标文件夹}}
```
#### 列出一个目录和任何子目录的可读大小，最深可达 n 级:
```shell
du -h -d {{N}} {{目标文件夹}}
```
#### 列出当前目录子目录中所有.jpg 文件的可读大小，并在末尾显示累计总数:
```shell
du -ch */*.jpg
```
{% endraw %}