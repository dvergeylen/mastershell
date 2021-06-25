---
layout: default
title: "wat2wasm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wat2wasm">
  <a href="/en/common/wat2wasm.html">wat2wasm</a> <a href="#wat2wasm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert a file from the WebAssembly text format to the binary format.
> More information: <https://github.com/WebAssembly/wabt>.

#### Parse and check a file for errors:
```shell
wat2wasm {{file.wat}}
```
#### Write the output binary to a given file:
```shell
wat2wasm {{file.wat}} -o {{file.wasm}}
```
#### Display simplified representation of every byte:
```shell
wat2wasm -v {{file.wat}}
```
{% endraw %}