---
layout: default
title: "chgrp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chgrp">
  <a href="/en/common/chgrp.html">chgrp</a> <a href="#chgrp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change group ownership of files and directories.
> More information: <https://www.gnu.org/software/coreutils/chgrp>.

#### Change the owner group of a file/directory:
```shell
chgrp {{group}} {{path/to/file_or_directory}}
```
#### Recursively change the owner group of a directory and its contents:
```shell
chgrp -R {{group}} {{path/to/directory}}
```
#### Change the owner group of a symbolic link:
```shell
chgrp -h {{group}} {{path/to/symlink}}
```
#### Change the owner group of a file/directory to match a reference file:
```shell
chgrp --reference={{path/to/reference_file}} {{path/to/file_or_directory}}
```
{% endraw %}