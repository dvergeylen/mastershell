---
layout: default
title: "lvdisplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvdisplay">
  <a href="/en/linux/lvdisplay.html">lvdisplay</a> <a href="#lvdisplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about Logical Volume Manager (LVM) logical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvdisplay.8.html>.

#### Display information about all logical volumes:
```shell
sudo lvdisplay
```
#### Display information about all logical volumes in volume group vg1:
```shell
sudo lvdisplay {{vg1}}
```
#### Display information about logical volume lv1 in volume group vg1:
```shell
sudo lvdisplay {{vg1/lv1}}
```
{% endraw %}