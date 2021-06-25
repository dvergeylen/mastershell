---
layout: default
title: "chown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chown">
  <a href="/en/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change user and group ownership of files and directories.
> More information: <https://www.gnu.org/software/coreutils/chown>.

#### Change the owner user of a file/directory:
```shell
chown {{user}} {{path/to/file_or_directory}}
```
#### Change the owner user and group of a file/directory:
```shell
chown {{user}}:{{group}} {{path/to/file_or_directory}}
```
#### Recursively change the owner of a directory and its contents:
```shell
chown -R {{user}} {{path/to/directory}}
```
#### Change the owner of a symbolic link:
```shell
chown -h {{user}} {{path/to/symlink}}
```
#### Change the owner of a file/directory to match a reference file:
```shell
chown --reference={{path/to/reference_file}} {{path/to/file_or_directory}}
```
{% endraw %}