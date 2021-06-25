---
layout: default
title: "e2undo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="e2undo">
  <a href="/en/linux/e2undo.html">e2undo</a> <a href="#e2undo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Replay undo logs for an ext2/ext3/ext4 filesystem.
> This can be used to undo a failed operation by an e2fsprogs program.
> More information: <https://man7.org/linux/man-pages/man8/e2undo.8.html>.

#### Display information about a specific undo file:
```shell
e2undo -h {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Perform a dry-run and display the candidate blocks for replaying:
```shell
e2undo -nv {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Perform an undo operation:
```shell
e2undo {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Perform an undo operation and display verbose information:
```shell
e2undo -v {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Write the old contents of the block to an undo file before overwriting a file system block:
```shell
e2undo -z {{path/to/file.e2undo}} {{path/to/undo_file}} {{/dev/sdXN}}
```
{% endraw %}