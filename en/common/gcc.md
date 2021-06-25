---
layout: default
title: "gcc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gcc">
  <a href="/en/common/gcc.html">gcc</a> <a href="#gcc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Preprocess and compile C and C++ source files, then assemble and link them together.
> More information: <https://gcc.gnu.org>.

#### Compile multiple source files into executable:
```shell
gcc {{source1.c}} {{source2.c}} -o {{executable}}
```
#### Allow warnings, debug symbols in output:
```shell
gcc {{source.c}} -Wall -Og -o {{executable}}
```
#### Include libraries from a different path:
```shell
gcc {{source.c}} -o {{executable}} -I{{header_path}} -L{{library_path}} -l{{library_name}}
```
#### Compile source code into Assembler instructions:
```shell
gcc -S {{source.c}}
```
#### Compile source code without linking:
```shell
gcc -c {{source.c}}
```
{% endraw %}