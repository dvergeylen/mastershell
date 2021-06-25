---
layout: default
title: "gplusplus"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gplusplus">
  <a href="/pt_br/common/g++.html">gplusplus</a> <a href="#gplusplus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compilador de arquivos de código fonte C++.
> Parte do GCC (GNU Compiler Collection).
> Mais informações: <https://gcc.gnu.org>.

#### Compilar um arquivo de código fonte para um binário executável:
```shell
g++ {{arquivo_fonte.cpp}} -o {{arquivo_executável}}
```
#### Compilar mostrando todos os erros e avisos:
```shell
g++ {{arquivo_fonte.cpp}} -Wall -o {{arquivo_executável}}
```
#### Compilar utilizando um padrão específico da linguagem (C++98/C++11/C++14/C++17):
```shell
g++ {{arquivo_fonte.cpp}} -std={{standard_linguagem}} -o {{arquivo_executável}}
```
#### Compilar incluindo bibliotecas localizadas em um local diferente do arquivo de código fonte:
```shell
g++ {{arquivo_fonte.cpp}} -o {{arquivo_executável}} -I{{caminho/para/header}} -L{{caminho/para/biblioteca}} -l{{nome_biblioteca}}
```
{% endraw %}