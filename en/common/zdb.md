---
layout: default
title: "zdb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zdb">
  <a href="/en/common/zdb.html">zdb</a> <a href="#zdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ZFS debugger.

#### Show detailed configuration of all mounted ZFS zpools:
```shell
zdb
```
#### Show detailed configuration for a specific ZFS pool:
```shell
zdb -C {{poolname}}
```
#### Show statistics about number, size and deduplication of blocks:
```shell
zdb -b {{poolname}}
```
{% endraw %}