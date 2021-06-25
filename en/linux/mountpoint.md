---
layout: default
title: "mountpoint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mountpoint">
  <a href="/en/linux/mountpoint.html">mountpoint</a> <a href="#mountpoint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Test if a directory is a filesystem mountpoint.

#### Check if a directory is a mountpoint:
```shell
mountpoint {{path/to/directory}}
```
#### Check if a directory is a mountpoint without showing any output:
```shell
mountpoint -q {{path/to/directory}}
```
#### Show major/minor numbers of a mountpoint's filesystem:
```shell
mountpoint --fs-devno {{path/to/directory}}
```
{% endraw %}