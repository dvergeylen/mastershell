---
layout: default
title: "wasm2wat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wasm2wat">
  <a href="/en/common/wasm2wat.html">wasm2wat</a> <a href="#wasm2wat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert a file from the WebAssembly binary format to the text format.

#### Convert a file to the text format and display it to the console:
```shell
wasm2wat {{file.wasm}}
```
#### Write the output to a given file:
```shell
wasm2wat {{file.wasm}} -o {{file.wat}}
```
{% endraw %}