---
layout: default
title: "lsb_release"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsb_release">
  <a href="/en/linux/lsb_release.html">lsb_release</a> <a href="#lsb_release"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provides certain LSB (Linux Standard Base) and distribution-specific information.

#### Print all available information:
```shell
lsb_release -a
```
#### Print a description (usually the full name) of the operating system:
```shell
lsb_release -d
```
#### Print only the operating system name (ID), suppressing the field name:
```shell
lsb_release -i -s
```
#### Print the release number and codename of the distribution, suppressing the field names:
```shell
lsb_release -rcs
```
{% endraw %}