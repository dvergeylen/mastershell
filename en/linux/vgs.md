---
layout: default
title: "vgs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vgs">
  <a href="/en/linux/vgs.html">vgs</a> <a href="#vgs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about volume groups.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/vgs.8.html>.

#### Display information about volume groups:
```shell
vgs
```
#### Display all volume groups:
```shell
vgs -a
```
#### Change default display to show more details:
```shell
vgs -v
```
#### Display only specific fields:
```shell
vgs -o {{field_name_1}},{{field_name_2}}
```
#### Append field to default display:
```shell
vgs -o +{{field_name}}
```
#### Suppress heading line:
```shell
vgs --noheadings
```
#### Use separator to separate fields:
```shell
vgs --separator =
```
{% endraw %}