---
layout: default
title: "clang"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clang">
  <a href="/it/common/clang.html">clang</a> <a href="#clang"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compilatore per sorgenti C, C++ ed Objective-C. Può essere usato come alternativa a GCC.
> Maggiori informazioni: <https://clang.llvm.org/docs/ClangCommandLineReference.html>.

#### Compila un file sorgente in un binario eseguibile:
```shell
clang {{sorgente_input.c}} -o {{eseguibile_output}}
```
#### Attiva l'output di tutti gli errori ed i warning:
```shell
clang {{sorgente_input.c}} -Wall -o {{eseguibile_output}}
```
#### Includi librerie contenute in un percorso differente da quello del file di sorgente:
```shell
clang {{sorgente_input.c}} -o {{eseguibile_output}} -I{{percorso_header}} -L{{percorso_librerie}} -l{{nome_libreria}}
```
#### Compila codice sorgente in IR LLVM (Intermediate Representation):
```shell
clang -S -emit-llvm {{file.c}} -o {{file.ll}}
```
{% endraw %}