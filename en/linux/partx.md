---
layout: default
title: "partx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="partx">
  <a href="/en/linux/partx.html">partx</a> <a href="#partx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Parse a partition table and tell the kernel about it.
> More information: <https://man7.org/linux/man-pages/man8/partx.8.html>.

#### List the partitions on a block device or disk image:
```shell
sudo partx --list {{path/to/device_or_disk_image}}
```
#### Add all the partitions found in a given block device to the kernel:
```shell
sudo partx --add --verbose {{path/to/device_or_disk_image}}
```
#### Delete all the partitions found from the kernel (does not alter partitions on disk):
```shell
sudo partx --delete {{path/to/device_or_disk_image}}
```
{% endraw %}