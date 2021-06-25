---
layout: default
title: "lvs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lvs">
  <a href="/en/linux/lvs.html">lvs</a> <a href="#lvs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about logical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvs.8.html>.

#### Display information about logical volumes:
```shell
lvs
```
#### Display all logical volumes:
```shell
lvs -a
```
#### Change default display to show more details:
```shell
lvs -v
```
#### Display only specific fields:
```shell
lvs -o {{field_name_1}},{{field_name_2}}
```
#### Append field to default display:
```shell
lvs -o +{{field_name}}
```
#### Suppress heading line:
```shell
lvs --noheadings
```
#### Use a separator to separate fields:
```shell
lvs --separator {{=}}
```
{% endraw %}