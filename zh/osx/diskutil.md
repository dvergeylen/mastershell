---
layout: default
title: "diskutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diskutil">
  <a href="/zh/osx/diskutil.html">diskutil</a> <a href="#diskutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于管理本地磁盘和卷的实用程序.

#### 列出所有当前可用的磁盘、分区和已装入的卷:
```shell
diskutil list
```
#### 修复卷的文件系统数据结构:
```shell
diskutil repairVolume {{目标卷文件}}
```
#### 卸载卷:
```shell
diskutil unmountDisk {{目标卷文件}}
```
#### 弹出 CD/DVD （先卸载）:
```shell
diskutil eject {{/dev/ 光驱文件名}}
```
{% endraw %}