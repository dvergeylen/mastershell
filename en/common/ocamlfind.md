---
layout: default
title: "ocamlfind"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ocamlfind">
  <a href="/en/common/ocamlfind.html">ocamlfind</a> <a href="#ocamlfind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The findlib package manager for OCaml.
> Simplifies linking executables with external libraries.
> More information: <http://projects.camlcity.org/projects/findlib.html>.

#### Compile a source file to a native binary and link with packages:
```shell
ocamlfind ocamlopt -package {{package1}},{{package2}} -linkpkg -o {{executable}} {{source_file.ml}}
```
#### Compile a source file to a bytecode binary and link with packages:
```shell
ocamlfind ocamlc -package {{package1}},{{package2}} -linkpkg -o {{executable}} {{source_file.ml}}
```
#### Cross-compile for a different platform:
```shell
ocamlfind -toolchain {{cross-toolchain}} ocamlopt -o {{executable}} {{source_file.ml}}
```
{% endraw %}