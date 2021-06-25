---
layout: default
title: "genkernel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="genkernel">
  <a href="/en/linux/genkernel.html">genkernel</a> <a href="#genkernel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gentoo Linux utility to compile and install kernels.

#### Automatically compile and install a generic kernel:
```shell
sudo genkernel all
```
#### Build and install the bzImage|initramfs|kernel|ramdisk only:
```shell
sudo genkernel {{bzImage|initramfs|kernel|ramdisk}}
```
#### Apply changes to the kernel configuration before compiling and installing:
```shell
sudo genkernel --menuconfig all
```
#### Generate a kernel with a custom name:
```shell
sudo genkernel --kernname={{custom_name}} all
```
#### Use a kernel source outside of the default directory `/usr/src/linux`:
```shell
sudo genkernel --kerneldir={{path/to/directory}} all
```
{% endraw %}