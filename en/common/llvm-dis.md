---
layout: default
title: "llvm-dis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="llvm-dis">
  <a href="/en/common/llvm-dis.html">llvm-dis</a> <a href="#llvm-dis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts LLVM bitcode files into human-readable LLVM Intermediate Representation (IR).
> More information: <https://www.llvm.org/docs/CommandGuide/llvm-dis.html>.

#### Convert a bitcode file as LLVM IR and write the result to stdout:
```shell
llvm-dis {{path/to/input.bc}} -o -
```
#### Convert a bitcode file to an LLVM IR file with the same filename:
```shell
llvm-dis {{path/to/file.bc}}
```
#### Convert a bitcode file to LLVM IR, writing the result to the specified file:
```shell
llvm-dis {{path/to/input.bc}} -o {{path/to/output.ll}}
```
{% endraw %}