---
layout: default
title: "blkid"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="blkid">
  <a href="/en/linux/blkid.html">blkid</a> <a href="#blkid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lists all recognized partitions and their Universally Unique Identifier (UUID).

#### List all partitions:
```shell
sudo blkid
```
#### List all partitions in a table, including current mountpoints:
```shell
sudo blkid -o list
```
{% endraw %}