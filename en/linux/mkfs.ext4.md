---
layout: default
title: "mkfs.ext4"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.ext4">
  <a href="/en/linux/mkfs.ext4.html">mkfs.ext4</a> <a href="#mkfs.ext4"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an ext4 filesystem inside a partition.

#### Create an ext4 filesystem inside partition 1 on device b (`sdb1`):
```shell
sudo mkfs.ext4 {{/dev/sdb1}}
```
#### Create an ext4 filesystem with a volume-label:
```shell
sudo mkfs.ext4 -L {{volume_label}} {{/dev/sdb1}}
```
{% endraw %}