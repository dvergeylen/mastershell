---
layout: default
title: "nasm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nasm">
  <a href="/en/common/nasm.html">nasm</a> <a href="#nasm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Netwide Assembler, a portable 80x86 assembler.
> More information: <https://nasm.us>.

#### Assemble `source.asm` into a binary file `source`, in the (default) raw binary format:
```shell
nasm {{source.asm}}
```
#### Assemble `source.asm` into a binary file `output_file`, in the specified format:
```shell
nasm -f {{format}} {{source.asm}} -o {{output_file}}
```
#### List valid output formats (along with basic nasm help):
```shell
nasm -hf
```
#### Assemble and generate an assembly listing file:
```shell
nasm -l {{list_file}} {{source.asm}}
```
#### Add a directory (must be written with trailing slash) to the include file search path before assembling:
```shell
nasm -i {{path/to/include_dir/}} {{source.asm}}
```
{% endraw %}