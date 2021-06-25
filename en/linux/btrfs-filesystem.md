---
layout: default
title: "btrfs filesystem"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs-filesystem">
  <a href="/en/linux/btrfs-filesystem.html">btrfs filesystem</a> <a href="#btrfs-filesystem"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage btrfs filesystems.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-filesystem>.

#### Show filesystem usage (optionally run as root to show detailed information):
```shell
btrfs filesystem usage {{path/to/btrfs_mount}}
```
#### Show usage by individual devices:
```shell
sudo btrfs filesystem show {{path/to/btrfs_mount}}
```
#### Defragment a single file on a btrfs filesystem (avoid while a deduplication agent is running):
```shell
sudo btrfs filesystem defragment -v {{path/to/file}}
```
#### Defragment a directory recursively (does not cross subvolume boundaries):
```shell
sudo btrfs filesystem defragment -v -r {{path/to/directory}}
```
#### Force syncing unwritten data blocks to disk(s):
```shell
sudo btrfs filesystem sync {{path/to/btrfs_mount}}
```
#### Summarize disk usage for the files in a directory recursively:
```shell
sudo btrfs filesystem du --summarize {{path/to/directory}}
```
{% endraw %}