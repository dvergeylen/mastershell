---
layout: default
title: "pvdisplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pvdisplay">
  <a href="/en/linux/pvdisplay.html">pvdisplay</a> <a href="#pvdisplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about Logical Volume Manager (LVM) physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvdisplay.8.html>.

#### Display information about all physical volumes:
```shell
sudo pvdisplay
```
#### Display information about the physical volume on drive `/dev/sdXY`:
```shell
sudo pvdisplay {{/dev/sdXY}}
```
{% endraw %}