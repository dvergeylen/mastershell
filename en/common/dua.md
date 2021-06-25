---
layout: default
title: "dua"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dua">
  <a href="/en/common/dua.html">dua</a> <a href="#dua"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dua (Disk Usage Analyzer) is a tool to conveniently learn about the usage of disk space of a given directory.
> More information: <https://github.com/Byron/dua-cli>.

#### Analyze specific directory:
```shell
dua {{path/to/directory}}
```
#### Display apparent size instead of disk usage:
```shell
dua --apparent-size
```
#### Count hard-linked files each time they are seen:
```shell
dua --count-hard-links
```
#### Aggregate the consumed space of one or more directories or files:
```shell
dua aggregate
```
#### Launch the terminal user interface:
```shell
dua interactive
```
#### Format printing byte counts:
```shell
dua --format {{metric|binary|bytes|GB|GiB|MB|MiB}}
```
#### Set the number of threads to be used:
```shell
dua --threads {{count}}
```
{% endraw %}