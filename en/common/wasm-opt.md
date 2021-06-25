---
layout: default
title: "wasm-opt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wasm-opt">
  <a href="/en/common/wasm-opt.html">wasm-opt</a> <a href="#wasm-opt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimize WebAssembly binary files.

#### Apply default optimizations and write to a given file:
```shell
wasm-opt -O {{input.wasm}} -o {{output.wasm}}
```
#### Apply all optimizations and write to a given file (takes more time, but generates optimal code):
```shell
wasm-opt -O4 {{input.wasm}} -o {{output.wasm}}
```
#### Optimize a file for size:
```shell
wasm-opt -Oz {{input.wasm}} -o {{output.wasm}}
```
#### Print the textual representation of the binary to console:
```shell
wasm-opt {{input.wasm}} --print
```
{% endraw %}