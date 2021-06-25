---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/en/linux/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files and directories.
> More information: <https://www.gnu.org/software/coreutils/cp>.

#### Copy a file to another location:
```shell
cp {{path/to/source_file.ext}} {{path/to/target_file.ext}}
```
#### Copy a file into another directory, keeping the filename:
```shell
cp {{path/to/source_file.ext}} {{path/to/target_parent_directory}}
```
#### Recursively copy a directory's contents to another location (if the destination exists, the directory is copied inside it):
```shell
cp -r {{path/to/source_directory}} {{path/to/target_directory}}
```
#### Copy a directory recursively, in verbose mode (shows files as they are copied):
```shell
cp -vr {{path/to/source_directory}} {{path/to/target_directory}}
```
#### Copy text files to another location, in interactive mode (prompts user before overwriting):
```shell
cp -i {{*.txt}} {{path/to/target_directory}}
```
#### Follow symbolic links before copying:
```shell
cp -L {{link}} {{path/to/target_directory}}
```
#### Use the full path of source files, creating any missing intermediate directories when copying:
```shell
cp --parents {{source/path/to/file}} {{path/to/target_file}}
```
{% endraw %}