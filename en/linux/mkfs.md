---
layout: default
title: "mkfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs">
  <a href="/en/linux/mkfs.html">mkfs</a> <a href="#mkfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build a Linux filesystem on a hard disk partition.
> This command is deprecated in favor of filesystem specific mkfs.<type> utils.

#### Build a Linux ext2 filesystem on a partition:
```shell
mkfs {{path/to/partition}}
```
#### Build a filesystem of a specified type:
```shell
mkfs -t {{ext4}} {{path/to/partition}}
```
#### Build a filesystem of a specified type and check for bad blocks:
```shell
mkfs -c -t {{ntfs}} {{path/to/partition}}
```
{% endraw %}