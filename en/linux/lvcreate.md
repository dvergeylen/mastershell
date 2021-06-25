---
layout: default
title: "lvcreate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvcreate">
  <a href="/en/linux/lvcreate.html">lvcreate</a> <a href="#lvcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a logical volume in an existing volume group. A volume group is a collection of logical and physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvcreate.8.html>.

#### Create a logical volume of 10 gigabytes in the volume group vg1:
```shell
lvcreate -L {{10G}} {{vg1}}
```
#### Create a 1500 megabyte linear logical volume named mylv in the volume group vg1:
```shell
lvcreate -L {{1500}} -n {{mylv}} {{vg1}}
```
#### Create a logical volume called mylv that uses 60% of the total space in volume group vg1:
```shell
lvcreate -l {{60%VG}} -n {{mylv}} {{vg1}}
```
#### Create a logical volume called mylv that uses all of the unallocated space in the volume group vg1:
```shell
lvcreate -l {{100%FREE}} -n {{mylv}} {{vg1}}
```
{% endraw %}