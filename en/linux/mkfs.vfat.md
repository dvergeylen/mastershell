---
layout: default
title: "mkfs.vfat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.vfat">
  <a href="/en/linux/mkfs.vfat.html">mkfs.vfat</a> <a href="#mkfs.vfat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an MS-DOS filesystem inside a partition.

#### Create a vfat filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.vfat {{/dev/sdb1}}
```
#### Create filesystem with a volume-name:
```shell
mkfs.vfat -n {{volume_name}} {{/dev/sdb1}}
```
#### Create filesystem with a volume-id:
```shell
mkfs.vfat -i {{volume_id}} {{/dev/sdb1}}
```
#### Use 5 instead of 2 file allocation tables:
```shell
mkfs.vfat -f 5 {{/dev/sdb1}}
```
{% endraw %}