---
layout: default
title: "btrfs subvolume"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs-subvolume">
  <a href="/zh/linux/btrfs-subvolume.html">btrfs subvolume</a> <a href="#btrfs-subvolume"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 btrfs 子卷和快照。
> 更多信息：<https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-subvolume>。

#### 创建一个新的空子卷：
```shell
sudo btrfs subvolume create {{指向新子卷的路径}}
```
#### 列出指定文件系统中的所有子卷和快照：
```shell
sudo btrfs subvolume list {{指向 btrfs 文件系统的路径}}
```
#### 删除一个子卷：
```shell
sudo btrfs subvolume delete {{指向子卷的路径}}
```
#### 创建现有子卷的只读快照：
```shell
sudo btrfs subvolume snapshot -r {{指向源子卷的路径}} {{指向目标的路径}}
```
#### 创建现有子卷的读写快照：
```shell
sudo btrfs subvolume snapshot {{指向源子卷的路径}} {{指向目标的路径}}
```
#### 显示有关子卷的详细信息：
```shell
sudo btrfs subvolume show {{指向子卷的路径}}
```
{% endraw %}