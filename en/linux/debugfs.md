---
layout: default
title: "debugfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="debugfs">
  <a href="/en/linux/debugfs.html">debugfs</a> <a href="#debugfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive ext2/ext3/ext4 filesystem debugger.

#### Open the filesystem in read only mode:
```shell
debugfs {{/dev/sdXN}}
```
#### Open the filesystem in read write mode:
```shell
debugfs -w {{/dev/sdXN}}
```
#### Read commands from a specified file, execute them and then exit:
```shell
debugfs -f {{path/to/cmd_file}} {{/dev/sdXN}}
```
#### View the filesystem stats in debugfs console:
```shell
stats
```
#### Close the filesystem:
```shell
close -a
```
#### List all available commands:
```shell
lr
```
{% endraw %}