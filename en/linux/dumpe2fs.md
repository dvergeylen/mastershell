---
layout: default
title: "dumpe2fs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dumpe2fs">
  <a href="/en/linux/dumpe2fs.html">dumpe2fs</a> <a href="#dumpe2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the super block and blocks group information for ext2/ext3/ext4 filesystems.
> Unmount the partition before running this command using `umount {{device}}`.
> More information: <https://manned.org/dumpe2fs>.

#### Display ext2, ext3 and ext4 filesystem information:
```shell
dumpe2fs {{/dev/sdXN}}
```
#### Display the blocks which are reserved as bad in the filesystem:
```shell
dumpe2fs -b {{/dev/sdXN}}
```
#### Force display filesystem information even with non-recognisable feature flags:
```shell
dumpe2fs -f {{/dev/sdXN}}
```
#### Only display the superblock information and not any of the block group descriptor detail information:
```shell
dumpe2fs -h {{/dev/sdXN}}
```
#### Print the detailed group information block numbers in hexadecimal format:
```shell
dumpe2fs -x {{/dev/sdXN}}
```
{% endraw %}