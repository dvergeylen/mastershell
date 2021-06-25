---
layout: default
title: "ltrace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ltrace">
  <a href="/en/linux/ltrace.html">ltrace</a> <a href="#ltrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic library calls of a process.
> More information: <https://manned.org/ltrace>.

#### Print (trace) library calls of a program binary:
```shell
ltrace ./{{program}}
```
#### Count library calls. Print a handy summary at the bottom:
```shell
ltrace -c {{path/to/program}}
```
#### Trace calls to malloc and free, omit those done by libc:
```shell
ltrace -e malloc+free-@libc.so* {{path/to/program}}
```
#### Write to file instead of terminal:
```shell
ltrace -o {{file}} {{path/to/program}}
```
{% endraw %}