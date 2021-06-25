---
layout: default
title: "head"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="head">
  <a href="/en/osx/head.html">head</a> <a href="#head"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Output the first part of files.

#### Output the first few lines of a file:
```shell
head -n {{count_of_lines}} {{filename}}
```
#### Output the first few bytes of a file:
```shell
head -c {{number_in_bytes}} {{filename}}
```
{% endraw %}