---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/en/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List directory contents.
> More information: <https://www.gnu.org/software/coreutils/ls>.

#### List files one per line:
```shell
ls -1
```
#### List all files, including hidden files:
```shell
ls -a
```
#### List all files, with trailing `/` added to directory names:
```shell
ls -F
```
#### Long format list (permissions, ownership, size, and modification date) of all files:
```shell
ls -la
```
#### Long format list with size displayed using human readable units (KiB, MiB, GiB):
```shell
ls -lh
```
#### Long format list sorted by size (descending):
```shell
ls -lS
```
#### Long format list of all files, sorted by modification date (oldest first):
```shell
ls -ltr
```
#### Only list directories:
```shell
ls -d {{*/}}
```
{% endraw %}