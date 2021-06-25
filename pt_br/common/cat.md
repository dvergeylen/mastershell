---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/pt_br/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe e concatena o conteúdo de arquivos.
> Mais informações: <https://www.gnu.org/software/coreutils/cat>.

#### Exibir o conteúdo de um arquivo no terminal:
```shell
cat {{arquivo}}
```
#### Concatenar o conteúdo de vários arquivos em um arquivo de destino:
```shell
cat {{arquivo1}} {{arquivo2}} > {{arquivo_de_destino}}
```
#### Adicionar o conteúdo de vários arquivos ao final de um arquivo de destino:
```shell
cat {{arquivo1}} {{arquivo2}} >> {{arquivo_de_destino}}
```
#### Exibir o conteúdo de um arquivo no terminal numerando as linhas:
```shell
cat -n {{arquivo}}
```
{% endraw %}