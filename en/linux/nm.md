---
layout: default
title: "nm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nm">
  <a href="/en/linux/nm.html">nm</a> <a href="#nm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List symbol names in object files.

#### List global (extern) functions in a file (prefixed with T):
```shell
nm -g {{file.o}}
```
#### List only undefined symbols in a file:
```shell
nm -u {{file.o}}
```
#### List all symbols, even debugging symbols:
```shell
nm -a {{file.o}}
```
#### Demangle C++ symbols (make them readable):
```shell
nm --demangle {{file.o}}
```
{% endraw %}