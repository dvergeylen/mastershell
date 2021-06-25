---
layout: default
title: "clang-format"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clang-format">
  <a href="/en/common/clang-format.html">clang-format</a> <a href="#clang-format"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to auto-format C/C++/Java/JavaScript/Objective-C/Protobuf/C# code.
> More information: <https://clang.llvm.org/docs/ClangFormat.html>.

#### Format a file and print the result to stdout:
```shell
clang-format {{path/to/file}}
```
#### Format a file in-place:
```shell
clang-format -i {{path/to/file}}
```
#### Format a file using a predefined coding style:
```shell
clang-format --style={{LLVM|Google|Chromium|Mozilla|WebKit}} {{path/to/file}}
```
#### Format a file using the `.clang-format` file in one of the parent directories of the source file:
```shell
clang-format --style=file {{path/to/file}}
```
#### Generate a custom `.clang-format` file:
```shell
clang-format --style={{LLVM|Google|Chromium|Mozilla|WebKit}} --dump-config > {{.clang-format}}
```
{% endraw %}