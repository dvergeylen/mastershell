---
layout: default
title: "mkfs.fat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.fat">
  <a href="/en/linux/mkfs.fat.html">mkfs.fat</a> <a href="#mkfs.fat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an MS-DOS filesystem inside a partition.

#### Create a fat filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.fat {{/dev/sdb1}}
```
#### Create filesystem with a volume-name:
```shell
mkfs.fat -n {{volume_name}} {{/dev/sdb1}}
```
#### Create filesystem with a volume-id:
```shell
mkfs.fat -i {{volume_id}} {{/dev/sdb1}}
```
#### Use 5 instead of 2 file allocation tables:
```shell
mkfs.fat -f 5 {{/dev/sdb1}}
```
{% endraw %}