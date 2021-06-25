---
layout: default
title: "opt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="opt">
  <a href="/en/common/opt.html">opt</a> <a href="#opt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool that takes LLVM source files and runs specified optimizations and/or analyses on them.
> More information: <https://llvm.org/docs/CommandGuide/opt.html>.

#### Run an optimization or analysis on a bitcode file:
```shell
opt -{{passname}} {{path/to/file.bc}} -S -o {{file_opt.bc}}
```
#### Output the Control Flow Graph of a function to a `.dot` file:
```shell
opt {{-dot-cfg}} -S {{path/to/file.bc}} -disable-output
```
#### Optimize the program at level 2 and output the result to another file:
```shell
opt -O2 {{path/to/file.bc}} -S -o {{path/to/output_file.bc}}
```
{% endraw %}