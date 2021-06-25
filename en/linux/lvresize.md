---
layout: default
title: "lvresize"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvresize">
  <a href="/en/linux/lvresize.html">lvresize</a> <a href="#lvresize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvresize.8.html>.

#### Change the size of a logical volume to 120GB:
```shell
lvresize --size {{120G}} {{volume_group}}/{{logical_volume}}
```
#### Extend the size of a logical volume as well as the underlying filesystem by 120GB:
```shell
lvresize --size +{{120G}} --resizefs {{volume_group}}/{{logical_volume}}
```
#### Extend the size of a logical volume to 100% of the free physical volume space:
```shell
lvresize --size {{100}}%FREE {{volume_group}}/{{logical_volume}}
```
#### Reduce the size of a logical volume as well as the underlying filesystem by 120GB:
```shell
lvresize --size -{{120G}} --resizefs {{volume_group}}/{{logical_volume}}
```
{% endraw %}