---
layout: default
title: "udisksctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="udisksctl">
  <a href="/en/linux/udisksctl.html">udisksctl</a> <a href="#udisksctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line program used to interact with the udisksd daemon process.
> More information: <http://storaged.org/doc/udisks2-api/latest/udisksctl.1.html>.

#### Show high-level information about disk drives and block devices:
```shell
udisksctl status
```
#### Show detailed information about a device:
```shell
udisksctl info --block-device {{/dev/sdX}}
```
#### Show detailed information about a device partition:
```shell
udisksctl info --block-device {{/dev/sdXN}}
```
#### Mount a device partition and prints the mount point:
```shell
udisksctl mount --block-device {{/dev/sdXN}}
```
#### Unmount a device partition:
```shell
udisksctl unmount --block-device {{/dev/sdXN}}
```
#### Monitor the daemon for events:
```shell
udisksctl monitor
```
{% endraw %}