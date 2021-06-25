---
layout: default
title: "mkinitcpio"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkinitcpio">
  <a href="/en/linux/mkinitcpio.html">mkinitcpio</a> <a href="#mkinitcpio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generates initial ramdisk environments for booting the Linux kernel based on the specified preset(s).
> More information: <https://man.archlinux.org/man/mkinitcpio.8>.

#### Perform a dry run (print what would be done without actually doing it):
```shell
mkinitcpio
```
#### Generate a ramdisk environment based on the `linux` preset:
```shell
mkinitcpio --preset {{linux}}
```
#### Generate a ramdisk environment based on the `linux-lts` preset:
```shell
mkinitcpio --preset {{linux-lts}}
```
#### Generate ramdisk environments based on all existing presets (used to regenerate all the initramfs images after a change in `/etc/mkinitcpio.conf`):
```shell
mkinitcpio --allpresets
```
#### Generate an initramfs image using an alternative configuration file:
```shell
mkinitcpio --config {{path/to/mkinitcpio.conf}} --generate {{path/to/initramfs.img}}
```
#### Generate an initramfs image for a kernel other than the one currently running (the installed kernel releases can be found in `/usr/lib/modules/`):
```shell
mkinitcpio --kernel {{kernel_version}} --generate {{path/to/initramfs.img}}
```
#### List all available hooks:
```shell
mkinitcpio --listhooks
```
#### Display help for a specific hook:
```shell
mkinitcpio --hookhelp {{hook_name}}
```
{% endraw %}