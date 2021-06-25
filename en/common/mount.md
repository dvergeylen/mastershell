---
layout: default
title: "mount"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mount">
  <a href="/en/common/mount.html">mount</a> <a href="#mount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provides access to an entire filesystem in one directory.

#### Show all mounted filesystems:
```shell
mount
```
#### Mount a device to a directory:
```shell
mount -t {{filesystem_type}} {{path/to/device_file}} {{path/to/target_directory}}
```
#### Mount a CD-ROM device (with the filetype ISO9660) to `/cdrom` (readonly):
```shell
mount -t {{iso9660}} -o ro {{/dev/cdrom}} {{/cdrom}}
```
#### Mount all the filesystem defined in `/etc/fstab`:
```shell
mount -a
```
#### Mount a specific filesystem described in `/etc/fstab` (e.g. `/dev/sda1 /my_drive ext2 defaults 0 2`):
```shell
mount {{/my_drive}}
```
#### Mount a directory to another directory:
```shell
mount --bind {{path/to/old_dir}} {{path/to/new_dir}}
```
{% endraw %}