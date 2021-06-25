---
layout: default
title: "zramctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zramctl">
  <a href="/en/linux/zramctl.html">zramctl</a> <a href="#zramctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Setup and control zram devices.
> Use `mkfs` or `mkswap` to format zram devices to partitions.

#### Check if zram is enabled:
```shell
lsmod | grep -i zram
```
#### Enable zram with a dynamic number of devices (use `zramctl` to configure devices further):
```shell
sudo modprobe zram
```
#### Enable zram with exactly 2 devices:
```shell
sudo modprobe zram num_devices={{2}}
```
#### Find and initialise the next free zram device to a 2GB virtual drive using LZ4 compression:
```shell
sudo zramctl --find --size {{2GB}} --algorithm {{lz4}}
```
#### List currently initialised devices:
```shell
zramctl
```
{% endraw %}