---
layout: default
title: "sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sync">
  <a href="/en/common/sync.html">sync</a> <a href="#sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Flushes all pending write operations to the appropriate disks.
> More information: <https://www.gnu.org/software/coreutils/sync>.

#### Flush all pending write operations on all disks:
```shell
sync
```
#### Flush all pending write operations on a single file to disk:
```shell
sync {{path/to/file}}
```
{% endraw %}