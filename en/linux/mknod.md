---
layout: default
title: "mknod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mknod">
  <a href="/en/linux/mknod.html">mknod</a> <a href="#mknod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create block or character device special files.
> More information: <https://www.gnu.org/software/coreutils/mknod>.

#### Create a block device:
```shell
sudo mknod {{path/to/device_file}} b {{major_device_number}} {{minor_device_number}}
```
#### Create a character device:
```shell
sudo mknod {{path/to/device_file}} c {{major_device_number}} {{minor_device_number}}
```
#### Create a FIFO (queue) device:
```shell
sudo mknod {{path/to/device_file}} p
```
#### Create a device file with default SELinux security context:
```shell
sudo mknod -Z {{path/to/device_file}} {{type}} {{major_device_number}} {{minor_device_number}}
```
{% endraw %}