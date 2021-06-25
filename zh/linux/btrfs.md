---
layout: default
title: "btrfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs">
  <a href="/zh/linux/btrfs.html">btrfs</a> <a href="#btrfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一种基于写时复制（COW）原理的 Linux 文件系统。

#### 创建子卷：
```shell
sudo btrfs subvolume create {{指向子卷的路径}}
```
#### 列出子卷：
```shell
sudo btrfs subvolume list {{指向挂载点的路径}}
```
#### 显示空间使用情况信息：
```shell
sudo btrfs filesystem df {{指向挂载点的路径}}
```
#### 启用配额（quota）：
```shell
sudo btrfs quota enable {{指向子卷的路径}}
```
#### 显示配额（quota）：
```shell
sudo btrfs qgroup show {{指向子卷的路径}}
```
{% endraw %}