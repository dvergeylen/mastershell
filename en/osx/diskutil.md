---
layout: default
title: "diskutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diskutil">
  <a href="/en/osx/diskutil.html">diskutil</a> <a href="#diskutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to manage local disks and volumes.

#### List all currently available disks, partitions and mounted volumes:
```shell
diskutil list
```
#### Repair the filesystem data structures of a volume:
```shell
diskutil repairVolume {{/dev/diskX}}
```
#### Unmount a volume:
```shell
diskutil unmountDisk {{/dev/diskX}}
```
#### Eject a CD/DVD (unmount first):
```shell
diskutil eject {{/dev/disk1}}
```
{% endraw %}