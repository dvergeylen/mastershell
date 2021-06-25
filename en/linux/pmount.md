---
layout: default
title: "pmount"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pmount">
  <a href="/en/linux/pmount.html">pmount</a> <a href="#pmount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mount arbitrary hotpluggable devices as a normal user.
> More information: <https://manned.org/pmount>.

#### Mount a device below `/media/` (using device as mount point):
```shell
pmount {{/dev/to/block/device}}
```
#### Mount a device with a specific filesystem type to `/media/label`:
```shell
pmount --type {{filesystem}} {{/dev/to/block/device}} {{label}}
```
#### Mount a CD-ROM (filesystem type ISO9660) in read-only mode:
```shell
pmount --type {{iso9660}} --read-only {{/dev/cdrom}}
```
#### Mount an NTFS-formatted disk, forcing read-write access:
```shell
pmount --type {{ntfs}} --read-write {{/dev/sdX}}
```
#### Display all mounted removable devices:
```shell
pmount
```
{% endraw %}