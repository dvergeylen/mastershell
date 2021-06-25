---
layout: default
title: "umount"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="umount">
  <a href="/en/common/umount.html">umount</a> <a href="#umount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Unlink a filesystem from its mount point, making it no longer accessible.
> A filesystem cannot be unmounted when it is busy.

#### Unmount a filesystem, by passing the path to the source it is mounted from:
```shell
umount {{path/to/device_file}}
```
#### Unmount a filesystem, by passing the path to the target where it is mounted:
```shell
umount {{path/to/mounted_directory}}
```
#### Unmount all mounted filesystems (except the `proc` filesystem):
```shell
umount -a
```
{% endraw %}