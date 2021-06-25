---
layout: default
title: "diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diff">
  <a href="/en/common/diff.html">diff</a> <a href="#diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare files and directories.
> More information: <https://man7.org/linux/man-pages/man1/diff.1.html>.

#### Compare files (lists changes to turn `old_file` into `new_file`):
```shell
diff {{old_file}} {{new_file}}
```
#### Compare files, ignoring white spaces:
```shell
diff -w {{old_file}} {{new_file}}
```
#### Compare files, showing the differences side by side:
```shell
diff -y {{old_file}} {{new_file}}
```
#### Compare files, showing the differences in unified format (as used by `git diff`):
```shell
diff -u {{old_file}} {{new_file}}
```
#### Compare directories recursively (shows names for differing files/directories as well as changes made to files):
```shell
diff -r {{old_directory}} {{new_directory}}
```
#### Compare directories, only showing the names of files that differ:
```shell
diff -rq {{old_directory}} {{new_directory}}
```
{% endraw %}