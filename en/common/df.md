---
layout: default
title: "df"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="df">
  <a href="/en/common/df.html">df</a> <a href="#df"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gives an overview of the filesystem disk space usage.
> More information: <https://www.gnu.org/software/coreutils/df>.

#### Display all filesystems and their disk usage:
```shell
df
```
#### Display all filesystems and their disk usage in human readable form:
```shell
df -h
```
#### Display the filesystem and its disk usage containing the given file or directory:
```shell
df {{path/to/file_or_directory}}
```
#### Display statistics on the number of free inodes:
```shell
df -i
```
#### Display filesystems but exclude the specified types:
```shell
df -x {{squashfs}} -x {{tmpfs}}
```
{% endraw %}