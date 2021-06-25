---
layout: default
title: "fallocate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fallocate">
  <a href="/en/linux/fallocate.html">fallocate</a> <a href="#fallocate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reserve or deallocate disk space to files.
> The utility allocates space without zeroing.

#### Reserve a file taking up 700MB of disk space:
```shell
fallocate --length {{700M}} {{path/to/file}}
```
#### Shrink an already allocated file by 200MB:
```shell
fallocate --collapse-range --length {{200M}} {{path/to/file}}
```
#### Shrink 20MB of space after 100MB in a file:
```shell
fallocate --collapse-range --offset {{100M}} --length {{20M}} {{path/to/file}}
```
{% endraw %}