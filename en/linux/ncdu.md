---
layout: default
title: "ncdu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ncdu">
  <a href="/en/linux/ncdu.html">ncdu</a> <a href="#ncdu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disk usage analyzer with an ncurses interface.

#### Analyze the current working directory:
```shell
ncdu
```
#### Analyze a given directory:
```shell
ncdu {{path/to/directory}}
```
#### Save results to a file:
```shell
ncdu -o {{path/to/file}}
```
#### Exclude files that match a pattern, argument can be given multiple times to add more patterns:
```shell
ncdu --exclude '{{*.txt}}'
```
{% endraw %}