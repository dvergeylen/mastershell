---
layout: default
title: "fusermount"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fusermount">
  <a href="/en/common/fusermount.html">fusermount</a> <a href="#fusermount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mount and unmount FUSE filesystems.
> More information: <https://man.archlinux.org/man/fusermount.1>.

#### Unmount a FUSE filesystem:
```shell
fusermount -u {{path/to/mount_point}}
```
#### Unmount a FUSE filesystem as soon as it becomes unused:
```shell
fusermount -z {{path/to/mount_point}}
```
#### Display version:
```shell
fusermount --version
```
{% endraw %}