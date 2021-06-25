---
layout: default
title: "du"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="du">
  <a href="/en/osx/du.html">du</a> <a href="#du"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disk usage: estimate and summarize file and directory space usage.

#### List the sizes of a directory and any subdirectories, in the given unit (KB/MB/GB):
```shell
du -{{k|m|g}} {{path/to/directory}}
```
#### List the sizes of a directory and any subdirectories, in human-readable form (i.e. auto-selecting the appropriate unit for each size):
```shell
du -h {{path/to/directory}}
```
#### Show the size of a single directory, in human readable units:
```shell
du -sh {{path/to/directory}}
```
#### List the human-readable sizes of a directory and of all the files and directories within it:
```shell
du -ah {{path/to/directory}}
```
#### List the human-readable sizes of a directory and any subdirectories, up to N levels deep:
```shell
du -h -d {{N}} {{path/to/directory}}
```
#### List the human-readable size of all `.jpg` files in subdirectories of the current directory, and show a cumulative total at the end:
```shell
du -ch */*.jpg
```
{% endraw %}