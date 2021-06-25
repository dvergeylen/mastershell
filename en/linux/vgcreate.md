---
layout: default
title: "vgcreate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vgcreate">
  <a href="/en/linux/vgcreate.html">vgcreate</a> <a href="#vgcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create volume groups combining multiple mass-storage devices.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/vgcreate.8.html>.

#### Create a new volume group called vg1 using the `/dev/sda1` device:
```shell
vgcreate {{vg1}} {{/dev/sda1}}
```
#### Create a new volume group called vg1 using multiple devices:
```shell
vgcreate {{vg1}} {{/dev/sda1}} {{/dev/sdb1}} {{/dev/sdc1}}
```
{% endraw %}