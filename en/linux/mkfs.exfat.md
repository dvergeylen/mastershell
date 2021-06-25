---
layout: default
title: "mkfs.exfat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.exfat">
  <a href="/en/linux/mkfs.exfat.html">mkfs.exfat</a> <a href="#mkfs.exfat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an exfat filesystem inside a partition.

#### Create an exfat filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.exfat {{/dev/sdb1}}
```
#### Create filesystem with a volume-name:
```shell
mkfs.exfat -n {{volume_name}} {{/dev/sdb1}}
```
#### Create filesystem with a volume-id:
```shell
mkfs.exfat -i {{volume_id}} {{/dev/sdb1}}
```
{% endraw %}