---
layout: default
title: "mke2fs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mke2fs">
  <a href="/en/linux/mke2fs.html">mke2fs</a> <a href="#mke2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a Linux filesystem inside a partition.

#### Create an ext2 filesystem in partition 1 of device b (`sdb1`):
```shell
mkfs.ext2 {{/dev/sdb1}}
```
#### Create an ext3 filesystem in partition 1 of device b (`sdb1`):
```shell
mkfs.ext3 {{/dev/sdb1}}
```
#### Create an ext4 filesystem in partition 1 of device b (`sdb1`):
```shell
mkfs.ext4 {{/dev/sdb1}}
```
{% endraw %}