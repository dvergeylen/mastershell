---
layout: default
title: "lvremove"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvremove">
  <a href="/en/linux/lvremove.html">lvremove</a> <a href="#lvremove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove one or more logical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvremove.8.html>.

#### Remove a logical volume in a volume group:
```shell
sudo lvremove {{volume_group}}/{{logical_volume}}
```
#### Remove all logical volumes in a volume group:
```shell
sudo lvremove {{volume_group}}
```
{% endraw %}