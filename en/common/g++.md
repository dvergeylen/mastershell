---
layout: default
title: "g++"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="g++">
  <a href="/en/common/g++.html">g++</a> <a href="#g++"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compiles C++ source files.
> Part of GCC (GNU Compiler Collection).
> More information: <https://gcc.gnu.org>.

#### Compile a source code file into an executable binary:
```shell
g++ {{source.cpp}} -o {{output_executable}}
```
#### Display (almost) all errors and warnings:
```shell
g++ {{source.cpp}} -Wall -o {{output_executable}}
```
#### Choose a language standard to compile for(C++98/C++11/C++14/C++17):
```shell
g++ {{source.cpp}} -std={{language_standard}} -o {{output_executable}}
```
#### Include libraries located at a different path than the source file:
```shell
g++ {{source.cpp}} -o {{output_executable}} -I{{header_path}} -L{{library_path}} -l{{library_name}}
```
{% endraw %}