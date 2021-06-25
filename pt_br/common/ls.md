---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/pt_br/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Listar o conteúdo de um diretório.
> Mais informações: <https://www.gnu.org/software/coreutils/ls>.

#### Listar todos os arquivos, apresentando um arquivo por linha:
```shell
ls -1
```
#### Listar todos os arquivos, incluindo arquivos ocultos:
```shell
ls -a
```
#### Listar todos os arquivos, exibindo permissões, propriedade, tamanho e data de modificação:
```shell
ls -la
```
#### Listar todos os arquivos, apresentando o tamanho em medidas legíveis por humanos (KiB, MiB, GiB):
```shell
ls -lh
```
#### Listar todos os arquivos ordenados por tamanho (descendente):
```shell
ls -lS
```
#### Listar todos os arquivos ordenados por data de modificação (mais antigos primeiro):
```shell
ls -ltr
```
{% endraw %}