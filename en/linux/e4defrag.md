---
layout: default
title: "e4defrag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="e4defrag">
  <a href="/en/linux/e4defrag.html">e4defrag</a> <a href="#e4defrag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Defragment an ext4 filesystem.

#### Defragment the filesystem:
```shell
e4defrag {{/dev/sdXN}}
```
#### See how fragmented a filesystem is:
```shell
e4defrag -c {{/dev/sdXN}}
```
#### Print errors and the fragmentation count before and after each file:
```shell
e4defrag -v {{/dev/sdXN}}
```
{% endraw %}