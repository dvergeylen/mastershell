---
layout: default
title: "dir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dir">
  <a href="/pt_br/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Listar os conteúdos de um diretório.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/dir>.

#### Mostrar o conteúdo do diretório atual:
```shell
dir
```
#### Mostrar o conteúdo do diretório no caminho provido pelo usuário:
```shell
dir {{caminho/para/diretório}}
```
#### Mostrar o conteúdo do diretório atual, incluindo arquivos e pastas escondidas:
```shell
dir /A
```
#### Mostrar o conteúdo do diretório provido pelo usuário, incluindo arquivos e pastas escondidas:
```shell
dir {{caminho/para/diretório}} /A
```
{% endraw %}