---
layout: default
title: "lsusb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsusb">
  <a href="/en/linux/lsusb.html">lsusb</a> <a href="#lsusb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about USB buses and devices connected to them.

#### List all the USB devices available:
```shell
lsusb
```
#### List the USB hierarchy as a tree:
```shell
lsusb -t
```
#### List verbose information about USB devices:
```shell
lsusb --verbose
```
#### List detailed information about a USB device:
```shell
lsusb -D {{device}}
```
#### List devices with a specified vendor and product id only:
```shell
lsusb -d {{vendor}}:{{product}}
```
{% endraw %}