---
layout: default
title: "qemu-img"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qemu-img">
  <a href="/en/common/qemu-img.html">qemu-img</a> <a href="#qemu-img"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for Quick Emulator Virtual HDD image creation and manipulation.

#### Create disk image with a specific size (in gigabytes):
```shell
qemu-img create {{image_name.img}} {{gigabytes}}G
```
#### Show information about a disk image:
```shell
qemu-img info {{image_name.img}}
```
#### Increase or decrease image size:
```shell
qemu-img resize {{image_name.img}} {{gigabytes}}G
```
#### Dump the allocation state of every sector of the specified disk image:
```shell
qemu-img map {{image_name.img}}
```
#### Convert a VMware .vmdk disk image to a KVM .qcow2 disk image:
```shell
qemu-img convert -O qcow2 {{path/to/file/foo.vmdk}} {{path/to/file/foo.qcow2}}
```
{% endraw %}