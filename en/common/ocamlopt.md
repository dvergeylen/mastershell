---
layout: default
title: "ocamlopt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ocamlopt">
  <a href="/en/common/ocamlopt.html">ocamlopt</a> <a href="#ocamlopt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The OCaml native code compiler.
> Produces native executables, e.g. ELF on Linux.
> More information: <https://ocaml.org>.

#### Compile a source file:
```shell
ocamlopt -o {{path/to/binary}} {{path/to/source_file.ml}}
```
#### Compile with debugging enabled:
```shell
ocamlopt -g -o {{path/to/binary}} {{path/to/source_file.ml}}
```
{% endraw %}