---
layout: default
title: "fortune"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fortune">
  <a href="/en/common/fortune.html">fortune</a> <a href="#fortune"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print a random quotation (fortune-cookie style).
> More information: <https://man.archlinux.org/man/fortune.6>.

#### Print a quotation:
```shell
fortune
```
#### Print an offensive quotation:
```shell
fortune -o
```
#### Print a long quotation:
```shell
fortune -l
```
#### Print a short quotation:
```shell
fortune -s
```
#### List the available quotation database files:
```shell
fortune -f
```
#### Print a quotation from one of the database files listed by `fortune -f`:
```shell
fortune {{filename}}
```
{% endraw %}