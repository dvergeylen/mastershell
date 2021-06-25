---
layout: default
title: "bpytop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bpytop">
  <a href="/en/linux/bpytop.html">bpytop</a> <a href="#bpytop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic real-time information about running processes with graphs. Similar to `gtop` and `htop`.
> More information: <https://github.com/aristocratos/bpytop>.

#### Start bpytop:
```shell
bpytop
```
#### Start in minimal mode without memory and networking boxes:
```shell
bpytop -m
```
#### Show version:
```shell
bpytop -v
```
#### Toggle minimal mode:
```shell
m
```
#### Search for running programs or processes:
```shell
f
```
#### Change settings:
```shell
M
```
{% endraw %}