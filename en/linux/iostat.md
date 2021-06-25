---
layout: default
title: "iostat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iostat">
  <a href="/en/linux/iostat.html">iostat</a> <a href="#iostat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report statistics for devices and partitions.

#### Display a report of CPU and disk statistics since system startup:
```shell
iostat
```
#### Display a report of CPU and disk statistics with units converted to megabytes:
```shell
iostat -m
```
#### Display CPU statistics:
```shell
iostat -c
```
#### Display disk statistics with disk names (including LVM):
```shell
iostat -N
```
#### Display extended disk statistics with disk names for device "sda":
```shell
iostat -xN {{sda}}
```
#### Display incremental reports of CPU and disk statistics every 2 seconds:
```shell
iostat {{2}}
```
{% endraw %}