---
layout: default
title: "resize2fs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="resize2fs">
  <a href="/en/linux/resize2fs.html">resize2fs</a> <a href="#resize2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resize an ext2, ext3 or ext4 filesystem.
> Does not resize the underlying partition, and the filesystem must be unmounted.

#### Automatically resize a filesystem:
```shell
resize2fs {{/dev/sdXN}}
```
#### Resize the filesystem to a size of 40G, displaying a progress bar:
```shell
resize2fs -p {{/dev/sdXN}} {{40G}}
```
#### Shrink the filesystem to its minimum possible size:
```shell
resize2fs -M {{/dev/sdXN}}
```
{% endraw %}