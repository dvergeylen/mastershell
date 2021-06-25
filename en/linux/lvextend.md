---
layout: default
title: "lvextend"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvextend">
  <a href="/en/linux/lvextend.html">lvextend</a> <a href="#lvextend"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Increase the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvextend.8.html>.

#### Increase a volume's size to 120GB:
```shell
lvextend --size {{120G}} {{logical_volume}}
```
#### Increase a volume's size by 40GB as well as the underlying filesystem:
```shell
lvextend --size +{{40G}} -r {{logical_volume}}
```
#### Increase a volume's size to 100% of the free physical volume space:
```shell
lvextend --size {{100}}%FREE {{logical_volume}}
```
{% endraw %}