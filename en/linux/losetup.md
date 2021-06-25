---
layout: default
title: "losetup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="losetup">
  <a href="/en/linux/losetup.html">losetup</a> <a href="#losetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set up and control loop devices.

#### List loop devices with detailed info:
```shell
losetup -a
```
#### Attach a file to a given loop device:
```shell
sudo losetup /dev/{{loop}} /{{path/to/file}}
```
#### Attach a file to a new free loop device and scan the device for partitions:
```shell
sudo losetup --show --partscan -f /{{path/to/file}}
```
#### Attach a file to a read-only loop device:
```shell
sudo losetup --read-only /dev/{{loop}} /{{path/to/file}}
```
#### Detach all loop devices:
```shell
sudo losetup -D
```
#### Detach a given loop device:
```shell
sudo losetup -d /dev/{{loop}}
```
{% endraw %}