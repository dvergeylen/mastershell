---
layout: default
title: "hexdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hexdump">
  <a href="/en/linux/hexdump.html">hexdump</a> <a href="#hexdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An ASCII, decimal, hexadecimal, octal dump.

#### Print the hexadecimal representation of a file:
```shell
hexdump {{file}}
```
#### Display the input offset in hexadecimal and its ASCII representation in two columns:
```shell
hexdump -C {{file}}
```
#### Display the hexadecimal representation of a file, but interpret only n bytes of the input:
```shell
hexdump -C -n{{number_of_bytes}} {{file}}
```
{% endraw %}