---
layout: default
title: "mons"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mons">
  <a href="/en/linux/mons.html">mons</a> <a href="#mons"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to quickly manage two displays.
> More information: <https://github.com/Ventto/mons>.

#### Enable only the primary monitor:
```shell
mons -o
```
#### Enable only the secondary monitor:
```shell
mons -s
```
#### Duplicate the primary monitor onto the secondary monitor, using the resolution of the primary monitor:
```shell
mons -d
```
#### Mirror the primary monitor onto the secondary monitor, using the resolution of the secondary monitor:
```shell
mons -m
```
{% endraw %}