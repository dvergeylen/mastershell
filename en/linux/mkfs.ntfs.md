---
layout: default
title: "mkfs.ntfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.ntfs">
  <a href="/en/linux/mkfs.ntfs.html">mkfs.ntfs</a> <a href="#mkfs.ntfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a NTFS filesystem inside a partition.

#### Create a NTFS filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.ntfs {{/dev/sdb1}}
```
#### Create filesystem with a volume-label:
```shell
mkfs.ntfs -L {{volume_label}} {{/dev/sdb1}}
```
#### Create filesystem with specific UUID:
```shell
mkfs.ntfs -U {{UUID}} {{/dev/sdb1}}
```
{% endraw %}