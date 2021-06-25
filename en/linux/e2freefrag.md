---
layout: default
title: "e2freefrag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="e2freefrag">
  <a href="/en/linux/e2freefrag.html">e2freefrag</a> <a href="#e2freefrag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the free space fragmentation information for ext2/ext3/ext4 filesystems.
> More information: <https://manned.org/e2freefrag>.

#### Check how many free blocks are present as contiguous and aligned free space:
```shell
e2freefrag {{/dev/sdXN}}
```
#### Specify chunk size in kilobytes to print how many free chunks are available:
```shell
e2freefrag -c {{chunk_size_in_kb}} {{/dev/sdXN}}
```
{% endraw %}