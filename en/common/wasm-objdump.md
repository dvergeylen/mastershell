---
layout: default
title: "wasm-objdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wasm-objdump">
  <a href="/en/common/wasm-objdump.html">wasm-objdump</a> <a href="#wasm-objdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information from WebAssembly binaries.

#### Display the section headers of a given binary:
```shell
wasm-objdump -h {{file.wasm}}
```
#### Display the entire disassembled output of a given binary:
```shell
wasm-objdump -d {{file.wasm}}
```
#### Display the details of each section:
```shell
wasm-objdump --details {{file.wasm}}
```
#### Display the details of a given section:
```shell
wasm-objdump --section '{{import}}' --details {{file.wasm}}
```
{% endraw %}