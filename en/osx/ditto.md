---
layout: default
title: "ditto"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ditto">
  <a href="/en/osx/ditto.html">ditto</a> <a href="#ditto"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files and directories.

#### Overwrite contents of destination directory with contents of source directory:
```shell
ditto {{path/to/source}} {{path/to/destination}}
```
#### Print a line to the Terminal window for every file that's being copied:
```shell
ditto -V {{path/to/source}} {{path/to/destination}}
```
#### Copy a given file or directory, while retaining the original file permissions:
```shell
ditto -rsrc {{path/to/source}} {{path/to/destination}}
```
{% endraw %}