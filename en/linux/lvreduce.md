---
layout: default
title: "lvreduce"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvreduce">
  <a href="/en/linux/lvreduce.html">lvreduce</a> <a href="#lvreduce"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reduce the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvreduce.8.html>.

#### Reduce a volume's size to 120GB:
```shell
lvreduce --size {{120G}} {{logical_volume}}
```
#### Reduce a volume's size by 40GB as well as the underlying filesystem:
```shell
lvreduce --size -{{40G}} -r {{logical_volume}}
```
{% endraw %}