---
layout: default
title: "eject"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eject">
  <a href="/en/linux/eject.html">eject</a> <a href="#eject"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Eject cds, floppy disks and tape drives.

#### Display the default device:
```shell
eject -d
```
#### Eject the default device:
```shell
eject
```
#### Eject a specific device (the default order is cd-rom, scsi, floppy and tape):
```shell
eject {{/dev/cdrom}}
```
#### Toggle whether a device's tray is open or closed:
```shell
eject -T {{/dev/cdrom}}
```
#### Eject a cd drive:
```shell
eject -r {{/dev/cdrom}}
```
#### Eject a floppy drive:
```shell
eject -f {{/mnt/floppy}}
```
#### Eject a tape drive:
```shell
eject -q {{/mnt/tape}}
```
{% endraw %}