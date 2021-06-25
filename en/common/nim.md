---
layout: default
title: "nim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nim">
  <a href="/en/common/nim.html">nim</a> <a href="#nim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Nim compiler.
> Processes, compiles and links Nim language source files.
> More information: <https://nim-lang.org>.

#### Compile a source file:
```shell
nim compile {{file.nim}}
```
#### Compile and run a source file:
```shell
nim compile -r {{file.nim}}
```
#### Compile a source file with release optimizations enabled:
```shell
nim compile -d:release {{file.nim}}
```
#### Build a release binary optimized for low file size:
```shell
nim compile -d:release --opt:size {{file.nim}}
```
#### Generate HTML documentation for a module (output will be placed in the current directory):
```shell
nim doc {{file.nim}}
```
{% endraw %}