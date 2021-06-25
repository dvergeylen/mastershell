---
layout: default
title: "mkfs.cramfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.cramfs">
  <a href="/en/linux/mkfs.cramfs.html">mkfs.cramfs</a> <a href="#mkfs.cramfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a ROM filesystem inside a partition.

#### Create a ROM filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.cramfs {{/dev/sdb1}}
```
#### Create a ROM filesystem with a volume-name:
```shell
mkfs.cramfs -n {{volume_name}} {{/dev/sdb1}}
```
{% endraw %}