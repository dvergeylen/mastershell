---
layout: default
title: "lsscsi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsscsi">
  <a href="/en/linux/lsscsi.html">lsscsi</a> <a href="#lsscsi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List SCSI devices (or hosts) and their attributes.

#### List all SCSI devices:
```shell
lsscsi
```
#### List all SCSI devices with detailed attributes:
```shell
lsscsi -L
```
#### List all SCSI devices with human readable disk capacity:
```shell
lsscsi -s
```
{% endraw %}