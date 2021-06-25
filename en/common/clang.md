---
layout: default
title: "clang"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clang">
  <a href="/en/common/clang.html">clang</a> <a href="#clang"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compiler for C, C++, and Objective-C source files. Can be used as a drop-in replacement for GCC.
> More information: <https://clang.llvm.org/docs/ClangCommandLineReference.html>.

#### Compile a source code file into an executable binary:
```shell
clang {{input_source.c}} -o {{output_executable}}
```
#### Activate output of all errors and warnings:
```shell
clang {{input_source.c}} -Wall -o {{output_executable}}
```
#### Include libraries located at a different path than the source file:
```shell
clang {{input_source.c}} -o {{output_executable}} -I{{header_path}} -L{{library_path}} -l{{library_name}}
```
#### Compile source code into LLVM Intermediate Representation (IR):
```shell
clang -S -emit-llvm {{file.c}} -o {{file.ll}}
```
{% endraw %}