---
layout: default
title: "grub-install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grub-install">
  <a href="/en/linux/grub-install.html">grub-install</a> <a href="#grub-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install GRUB to a device.
> More information: <https://www.gnu.org/software/grub/manual/grub/html_node/Installing-GRUB-using-grub_002dinstall.html>.

#### Install GRUB on a BIOS system:
```shell
grub-install --target={{i386-pc}} {{path/to/device}}
```
#### Install GRUB on an UEFI system:
```shell
grub-install --target={{x86_64-efi}} --efi-directory={{path/to/efi_directory}} --bootloader-id={{GRUB}}
```
#### Install GRUB pre-loading specific modules:
```shell
grub-install --target={{x86_64-efi}} --efi-directory={{path/to/efi_directory}} --modules="{{part_gpt part_msdos}}"
```
{% endraw %}