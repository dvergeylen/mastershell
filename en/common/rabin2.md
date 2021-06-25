---
layout: default
title: "rabin2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rabin2">
  <a href="/en/common/rabin2.html">rabin2</a> <a href="#rabin2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get information about binary files (ELF, PE, Java CLASS, Mach-O) - symbols, sections, linked libraries, etc.
> Comes bundled with `radare2`.

#### Display general information about a binary (architecture, type, endianness):
```shell
rabin2 -I {{path/to/binary}}
```
#### Display linked libraries:
```shell
rabin2 -l {{path/to/binary}}
```
#### Display symbols imported from libraries:
```shell
rabin2 -i {{path/to/binary}}
```
#### Display strings contained in the binary:
```shell
rabin2 -z {{path/to/binary}}
```
#### Display the output in JSON:
```shell
rabin2 -j -I {{path/to/binary}}
```
{% endraw %}