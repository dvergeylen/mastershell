---
layout: default
title: "gcc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gcc">
  <a href="/pt_br/common/gcc.html">gcc</a> <a href="#gcc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compilador de arquivos de código fonte C e C++, efetuando também as fases de pré-processamento, assembling e linking.
> Mais informações: <https://gcc.gnu.org>.

#### Compilar múltiplos arquivos de código fonte, produzindo um arquivo executável:
```shell
gcc {{arquivo_fonte1.c}} {{arquivo_fonte2.c}} -o {{arquivo_executável}}
```
#### Habilitar avisos durante a compilação:
```shell
gcc {{arquivo_fonte.c}} -Wall -Og -o {{arquivo_executável}}
```
#### Incluir bibliotecas de um local diferente:
```shell
gcc {{arquivo_fonte.c}} -o {{arquivo_executável}} -I{{caminho/para/header}} -L{{caminho/para/biblioteca}} -l{{nome_biblioteca}}
```
#### Compilar o código fonte para instruções Assembler:
```shell
gcc -S {{arquivo_fonte.c}}
```
#### Compilar o código fonte sem efetuar a fase de linking:
```shell
gcc -c {{arquivo_fonte.c}}
```
{% endraw %}