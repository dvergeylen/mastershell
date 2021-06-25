---
layout: default
title: "tune2fs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tune2fs">
  <a href="/en/linux/tune2fs.html">tune2fs</a> <a href="#tune2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Adjust parameters of an ext2, ext3 or ext4 filesystem.
> May be used on mounted filesystems.

#### Set the max number of counts before a filesystem is checked to 2:
```shell
tune2fs -c {{2}} {{/dev/sdXN}}
```
#### Set the filesystem label to MY_LABEL:
```shell
tune2fs -L {{'MY_LABEL'}} {{/dev/sdXN}}
```
#### Enable discard and user-specified extended attributes for a filesystem:
```shell
tune2fs -o {{discard,user_xattr}} {{/dev/sdXN}}
```
#### Enable journaling for a filesystem:
```shell
tune2fs -o^{{nobarrier}} {{/dev/sdXN}}
```
{% endraw %}