---
layout: default
title: "zfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zfs">
  <a href="/en/common/zfs.html">zfs</a> <a href="#zfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage ZFS filesystems.

#### List all available zfs filesystems:
```shell
zfs list
```
#### Create a new ZFS filesystem:
```shell
zfs create {{pool_name/filesystem_name}}
```
#### Delete a ZFS filesystem:
```shell
zfs destroy {{pool_name/filesystem_name}}
```
#### Create a Snapshot of a ZFS filesystem:
```shell
zfs snapshot {{pool_name/filesystem_name}}@{{snapshot_name}}
```
#### Enable compression on a filesystem:
```shell
zfs set compression=on {{pool_name/filesystem_name}}
```
#### Change mountpoint for a filesystem:
```shell
zfs set mountpoint={{/my/mount/path}} {{pool_name/filesystem_name}}
```
{% endraw %}