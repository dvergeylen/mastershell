---
layout: default
title: "e2fsck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="e2fsck">
  <a href="/en/linux/e2fsck.html">e2fsck</a> <a href="#e2fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check a Linux ext2/ext3/ext4 filesystem. The filesystem should be unmounted at the time the command is run.

#### Check filesystem, reporting any damaged blocks:
```shell
e2fsck {{/dev/sdXN}}
```
#### Check filesystem and automatically repair any damaged blocks:
```shell
e2fsck -p {{/dev/sdXN}}
```
#### Check filesystem in read only mode:
```shell
e2fsck -c {{/dev/sdXN}}
```
{% endraw %}