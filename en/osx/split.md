---
layout: default
title: "split"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="split">
  <a href="/en/osx/split.html">split</a> <a href="#split"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Split a file into pieces.

#### Split a file, each split having 10 lines (except the last split):
```shell
split -l {{10}} {{filename}}
```
#### Split a file by a regular expression. The matching line will be the first line of the next output file:
```shell
split -p {{cat|^[dh]og}} {{filename}}
```
#### Split a file with 512 bytes in each split (except the last split; use 512k for kilobytes and 512m for megabytes):
```shell
split -b {{512}} {{filename}}
```
{% endraw %}