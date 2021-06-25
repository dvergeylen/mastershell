---
layout: default
title: "ln"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ln">
  <a href="/en/common/ln.html">ln</a> <a href="#ln"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates links to files and directories.
> More information: <https://www.gnu.org/software/coreutils/ln>.

#### Create a symbolic link to a file or directory:
```shell
ln -s {{/path/to/file_or_directory}} {{path/to/symlink}}
```
#### Overwrite an existing symbolic link to point to a different file:
```shell
ln -sf {{/path/to/new_file}} {{path/to/symlink}}
```
#### Create a hard link to a file:
```shell
ln {{/path/to/file}} {{path/to/hardlink}}
```
{% endraw %}