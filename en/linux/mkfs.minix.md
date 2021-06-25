---
layout: default
title: "mkfs.minix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.minix">
  <a href="/en/linux/mkfs.minix.html">mkfs.minix</a> <a href="#mkfs.minix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a Minix filesystem inside a partition.

#### Create a Minix filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.minix {{/dev/sdb1}}
```
{% endraw %}