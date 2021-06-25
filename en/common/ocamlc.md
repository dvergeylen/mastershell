---
layout: default
title: "ocamlc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ocamlc">
  <a href="/en/common/ocamlc.html">ocamlc</a> <a href="#ocamlc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The OCaml bytecode compiler.
> Produces executables runnable by the OCaml interpreter.
> More information: <https://ocaml.org>.

#### Create a binary from a source file:
```shell
ocamlc {{path/to/source_file.ml}}
```
#### Create a named binary from a source file:
```shell
ocamlc -o {{path/to/binary}} {{path/to/source_file.ml}}
```
#### Automatically generate a module signature (interface) file:
```shell
ocamlc -i {{path/to/source_file.ml}}
```
{% endraw %}