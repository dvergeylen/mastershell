---
layout: default
title: "jhat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jhat">
  <a href="/en/common/jhat.html">jhat</a> <a href="#jhat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java Heap Analysis Tool.

#### Analyze a heap dump (from jmap), view via http on port 7000:
```shell
jhat {{dump_file.bin}}
```
#### Analyze a heap dump, specifying an alternate port for the http server:
```shell
jhat -p {{port}} {{dump_file.bin}}
```
#### Analyze a dump letting jhat use up to 8GB RAM (2-4x dump size recommended):
```shell
jhat -J-mx8G {{dump_file.bin}}
```
{% endraw %}