---
layout: default
title: "split"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="split">
  <a href="/en/common/split.html">split</a> <a href="#split"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Split a file into pieces.
> More information: <https://www.gnu.org/software/coreutils/split>.

#### Split a file, each split having 10 lines (except the last split):
```shell
split -l {{10}} {{filename}}
```
#### Split a file into 5 files. File is split such that each split has same size (except the last split):
```shell
split -n {{5}} {{filename}}
```
#### Split a file with 512 bytes in each split (except the last split; use 512k for kilobytes and 512m for megabytes):
```shell
split -b {{512}} {{filename}}
```
#### Split a file with at most 512 bytes in each split without breaking lines:
```shell
split -C {{512}} {{filename}}
```
{% endraw %}