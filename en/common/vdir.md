---
layout: default
title: "vdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vdir">
  <a href="/en/common/vdir.html">vdir</a> <a href="#vdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List directory contents.
> Drop-in replacement for `ls -l`.
> More information: <https://www.gnu.org/software/coreutils/vdir>.

#### List files and directories in the current directory, one per line, with details:
```shell
vdir
```
#### List with sizes displayed in human readable units (KB, MB, GB):
```shell
vdir -h
```
#### List including hidden files (starting with a dot):
```shell
vdir -a
```
#### List files and directories sorting entries by size (largest first):
```shell
vdir -S
```
#### List files and directories sorting entries by modification time (newest first):
```shell
vdir -t
```
#### List grouping directories first:
```shell
vdir --group-directories-first
```
#### Recursively list all files and directories in a specific directory:
```shell
vdir --recursive {{path/to/directory}}
```
{% endraw %}