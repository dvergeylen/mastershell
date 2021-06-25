---
layout: default
title: "btrfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs">
  <a href="/en/linux/btrfs.html">btrfs</a> <a href="#btrfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A filesystem based on the copy-on-write (COW) principle for Linux.

#### Create subvolume:
```shell
sudo btrfs subvolume create {{path/to/subvolume}}
```
#### List subvolumes:
```shell
sudo btrfs subvolume list {{path/to/mount_point}}
```
#### Show space usage information:
```shell
sudo btrfs filesystem df {{path/to/mount_point}}
```
#### Enable quota:
```shell
sudo btrfs quota enable {{path/to/subvolume}}
```
#### Show quota:
```shell
sudo btrfs qgroup show {{path/to/subvolume}}
```
{% endraw %}