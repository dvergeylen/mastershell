---
layout: default
title: "lvm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvm">
  <a href="/en/linux/lvm.html">lvm</a> <a href="#lvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage physical volumes, volume groups, and logical volumes using the Logical Volume Manager (LVM) interactive shell.
> More information: <https://man7.org/linux/man-pages/man8/lvm.8.html>.

#### Start the Logical Volume Manager interactive shell:
```shell
sudo lvm
```
#### List the Logical Volume Manager commands:
```shell
sudo lvm help
```
#### Initialize a drive or partition to be used as a physical volume:
```shell
sudo lvm pvcreate {{/dev/sdXY}}
```
#### Display information about physical volumes:
```shell
sudo lvm pvdisplay
```
#### Create a volume group called vg1 from the physical volume on `/dev/sdXY`:
```shell
sudo lvm vgcreate {{vg1}} {{/dev/sdXY}}
```
#### Display information about volume groups:
```shell
sudo lvm vgdisplay
```
#### Create a logical volume with size 10G from volume group vg1:
```shell
sudo lvm lvcreate -L {{10G}} {{vg1}}
```
#### Display information about logical volumes:
```shell
sudo lvm lvdisplay
```
{% endraw %}