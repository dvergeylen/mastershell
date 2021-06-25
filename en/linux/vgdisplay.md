---
layout: default
title: "vgdisplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vgdisplay">
  <a href="/en/linux/vgdisplay.html">vgdisplay</a> <a href="#vgdisplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about Logical Volume Manager (LVM) volume groups.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/vgdisplay.8.html>.

#### Display information about all volume groups:
```shell
sudo vgdisplay
```
#### Display information about volume group vg1:
```shell
sudo vgdisplay {{vg1}}
```
{% endraw %}