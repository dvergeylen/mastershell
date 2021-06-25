---
layout: default
title: "addr2line"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="addr2line">
  <a href="/en/linux/addr2line.html">addr2line</a> <a href="#addr2line"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert addresses of a binary into file names and line numbers.

#### Display the filename and line number of the source code from an instruction address of an executable:
```shell
addr2line --exe={{path/to/executable}} {{address}}
```
#### Display the function name, filename and line number:
```shell
addr2line --exe={{path/to/executable}} --functions {{address}}
```
#### Demangle the function name for C++ code:
```shell
addr2line --exe={{path/to/executable}} --functions --demangle {{address}}
```
{% endraw %}