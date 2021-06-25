---
layout: default
title: "wasm2c"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wasm2c">
  <a href="/en/common/wasm2c.html">wasm2c</a> <a href="#wasm2c"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert a file from the WebAssembly binary format to a C source file and header.

#### Convert a file to a C source file and header and display it to the console:
```shell
wasm2c {{file.wasm}}
```
#### Write the output to a given file (`file.h` gets additionally generated):
```shell
wasm2c {{file.wasm}} -o {{file.c}}
```
{% endraw %}