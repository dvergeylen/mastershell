---
layout: default
title: "btrfs subvolume"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs-subvolume">
  <a href="/en/linux/btrfs-subvolume.html">btrfs subvolume</a> <a href="#btrfs-subvolume"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage btrfs subvolumes and snapshots.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-subvolume>.

#### Create a new empty subvolume:
```shell
sudo btrfs subvolume create {{path/to/new_subvolume}}
```
#### List all subvolumes and snapshots in the specified filesystem:
```shell
sudo btrfs subvolume list {{path/to/btrfs_filesystem}}
```
#### Delete a subvolume:
```shell
sudo btrfs subvolume delete {{path/to/subvolume}}
```
#### Create a read-only snapshot of an existing subvolume:
```shell
sudo btrfs subvolume snapshot -r {{path/to/source_subvolume}} {{path/to/target}}
```
#### Create a read-write snapshot of an existing subvolume:
```shell
sudo btrfs subvolume snapshot {{path/to/source_subvolume}} {{path/to/target}}
```
#### Show detailed information about a subvolume:
```shell
sudo btrfs subvolume show {{path/to/subvolume}}
```
{% endraw %}