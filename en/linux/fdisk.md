---
layout: default
title: "fdisk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdisk">
  <a href="/en/linux/fdisk.html">fdisk</a> <a href="#fdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A program for managing partition tables and partitions on a hard disk.

#### List partitions:
```shell
fdisk -l
```
#### Start the partition manipulator:
```shell
fdisk {{/dev/sdX}}
```
{% endraw %}