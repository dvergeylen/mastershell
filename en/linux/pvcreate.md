---
layout: default
title: "pvcreate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pvcreate">
  <a href="/en/linux/pvcreate.html">pvcreate</a> <a href="#pvcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Initialize a disk or partition for use as a physical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvcreate.8.html>.

#### Initialize the `/dev/sda1` volume for use by LVM:
```shell
pvcreate {{/dev/sda1}}
```
#### Force the creation without any confirmation prompts:
```shell
pvcreate --force {{/dev/sda1}}
```
{% endraw %}