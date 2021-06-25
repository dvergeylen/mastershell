---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/pt_br/windows/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe uma árvore gráfica da estrutura do diretório no caminho.
> Mais informações: <https://docs.microsoft.com/windows-server/administration/windows-commands/tree>.

#### Exibe a árvore para o diretório atual:
```shell
tree
```
#### Exibe a árvore para o diretório específico:
```shell
tree {{caminho/para/diretório}}
```
#### Exibe a árvore para o diretório específico incluíndo arquivos:
```shell
tree {{caminho/para/diretório}} /f
```
#### Exibe a árvore usando caractéres ASCII:
```shell
tree {{caminho/para/diretório}} /a
```
{% endraw %}