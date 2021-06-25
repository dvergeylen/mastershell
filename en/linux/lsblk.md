---
layout: default
title: "lsblk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsblk">
  <a href="/en/linux/lsblk.html">lsblk</a> <a href="#lsblk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lists information about devices.

#### List all storage devices in a tree-like format:
```shell
lsblk
```
#### Also list empty devices:
```shell
lsblk -a
```
#### Print the SIZE column in bytes rather than in a human-readable format:
```shell
lsblk -b
```
#### Output info about filesystems:
```shell
lsblk -f
```
#### Use ASCII characters for tree formatting:
```shell
lsblk -i
```
#### Output info about block-device topology:
```shell
lsblk -t
```
#### Exclude the devices specified by the comma-separated list of major device numbers:
```shell
lsblk -e {{1,7}}
```
#### Display a customized summary using a comma-separated list of columns:
```shell
lsblk --output {{NAME}},{{SERIAL}},{{MODEL}},{{TRAN}},{{TYPE}},{{SIZE}},{{FSTYPE}},{{MOUNTPOINT}}
```
{% endraw %}