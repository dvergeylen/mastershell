---
layout: default
title: "btrfs device"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs-device">
  <a href="/en/linux/btrfs-device.html">btrfs device</a> <a href="#btrfs-device"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage devices in a btrfs filesystem.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-device>.

#### Add one or more devices to a btrfs filesystem:
```shell
sudo btrfs device add {{path/to/block_device1}} [{{path/to/block_device2}}] {{path/to/btrfs_filesystem}}
```
#### Remove a device from a btrfs filesystem:
```shell
sudo btrfs device remove {{path/to/device|device_id}} [{{...}}]
```
#### Display error statistics:
```shell
sudo btrfs device stats {{path/to/btrfs_filesystem}}
```
#### Scan all disks and inform the kernel of all detected btrfs filesystems:
```shell
sudo btrfs device scan --all-devices
```
#### Display detailed per-disk allocation statistics:
```shell
sudo btrfs device usage {{path/to/btrfs_filesystem}}
```
{% endraw %}