---
layout: default
title: "btrfs device"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs-device">
  <a href="/zh/linux/btrfs-device.html">btrfs device</a> <a href="#btrfs-device"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 btrfs 文件系统中的设备。
> 更多信息：<https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-device>。

#### 将一个或多个设备添加到 b​​trfs 文件系统中：
```shell
sudo btrfs device add {{指向设备1的路径}} [{{指向设备2的路径}}] {{指向 btrfs 文件系统的路径}}
```
#### 从 btrfs 文件系统中删除设备：
```shell
sudo btrfs device remove {{指向设备的路径|设备 ID}} [{{...}}]
```
#### 显示错误统计：
```shell
sudo btrfs device stats {{指向 btrfs 文件系统的路径}}
```
#### 扫描所有磁盘并将所有检测到的 btrfs 文件系统通知内核：
```shell
sudo btrfs device scan --all-devices
```
#### 显示详细的每个磁盘的空间分配统计信息：
```shell
sudo btrfs device usage {{指向 btrfs 文件系统的路径}}
```
{% endraw %}