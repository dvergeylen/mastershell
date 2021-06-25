---
layout: default
title: "qemu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qemu">
  <a href="/en/common/qemu.html">qemu</a> <a href="#qemu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generic machine emulator and virtualizer.
> Supports a large variety of CPU architectures.
> More information: <https://www.qemu.org>.

#### Boot from image emulating i386 architecture:
```shell
qemu-system-i386 -hda {{image_name.img}}
```
#### Boot from image emulating x64 architecture:
```shell
qemu-system-x86_64 -hda {{image_name.img}}
```
#### Boot QEMU instance with a live ISO image:
```shell
qemu-system-i386 -hda {{image_name.img}} -cdrom {{os_image.iso}} -boot d
```
#### Specify amount of RAM for instance:
```shell
qemu-system-i386 -m 256 -hda image_name.img -cdrom os-image.iso -boot d
```
#### Boot from physical device (e.g. from USB to test bootable medium):
```shell
qemu-system-i386 -hda /dev/{{storage_device}}
```
{% endraw %}