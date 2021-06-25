---
layout: default
title: "kpartx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kpartx">
  <a href="/en/linux/kpartx.html">kpartx</a> <a href="#kpartx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create device maps from partition tables.

#### Add partition mappings:
```shell
kpartx -a {{whole_disk.img}}
```
#### Delete partition mappings:
```shell
kpartx -d {{whole_disk.img}}
```
#### List partition mappings:
```shell
kpartx -l {{whole_disk.img}}
```
{% endraw %}