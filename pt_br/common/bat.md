---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/pt_br/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprimir e concatenar arquivos.
> Um clone do `cat` com realce de sintaxe e integração com Git.
> Mais informações: <https://github.com/sharkdp/bat>.

#### Imprimir o conteúdo de um arquivo para a saída padrão:
```shell
bat {{arquivo}}
```
#### Concatenar vários arquivos em um arquivo de destino:
```shell
bat {{caminho/para/arquivo1}} {{caminho/para/arquivo2}} > {{caminho/para/arquivo_destino}}
```
#### Numerar todas as linhas do output:
```shell
bat -n {{caminho/para/arquivo}}
```
#### Realçar a sintaxe em um arquivo JSON:
```shell
bat --language json {{caminho/para/arquivo.json}}
```
#### Mostrar todas as linguagens suportadas:
```shell
bat --list-languages
```
{% endraw %}