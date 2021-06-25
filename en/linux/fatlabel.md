---
layout: default
title: "fatlabel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fatlabel">
  <a href="/en/linux/fatlabel.html">fatlabel</a> <a href="#fatlabel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sets or gets the label of a FAT32 partition.

#### Get the label of a FAT32 partition:
```shell
fatlabel {{/dev/sda1}}
```
#### Set the label of a FAT32 partition:
```shell
fatlabel {{/dev/sdc3}} "{{new_label}}"
```
{% endraw %}