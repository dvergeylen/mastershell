---
layout: default
title: "pvs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pvs">
  <a href="/en/linux/pvs.html">pvs</a> <a href="#pvs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvs.8.html>.

#### Display information about physical volumes:
```shell
pvs
```
#### Display non-physical volumes:
```shell
pvs -a
```
#### Change default display to show more details:
```shell
pvs -v
```
#### Display only specific fields:
```shell
pvs -o {{field_name_1}},{{field_name_2}}
```
#### Append field to default display:
```shell
pvs -o +{{field_name}}
```
#### Suppress heading line:
```shell
pvs --noheadings
```
#### Use separator to separate fields:
```shell
pvs --separator {{special_character}}
```
{% endraw %}