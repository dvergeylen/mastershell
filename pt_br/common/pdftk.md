---
layout: default
title: "pdftk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdftk">
  <a href="/pt_br/common/pdftk.html">pdftk</a> <a href="#pdftk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Conjunto de utilitários para manipular arquivos PDF.
> Mais informações: <https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit>.

#### Extrair conjuntos de páginas de um arquivo PDF (páginas 1 a 3, 5 e 6 a 10) e guardá-las num novo arquivo:
```shell
pdftk {{arquivo.pdf}} cat {{1-3 5 6-10}} output {{novo_arquivo.pdf}}
```
#### Concatenar uma lista de arquivos PDF, guardando o resultado num novo arquivo:
```shell
pdftk {{arquivo1.pdf arquivo2.pdf arquivoN.pdf ...}} cat output {{novo_arquivo.pdf}}
```
#### Partir cada página de um arquivo PDF num arquivo separado, com um padrão para o nome dos novos arquivos:
```shell
pdftk {{arquivo.pdf}} burst output {{página_%d.pdf}}
```
#### Girar em 180° todas as páginas de um arquivo PDF:
```shell
pdftk {{arquivo.pdf}} cat {{1-endsouth}} output {{novo_arquivo.pdf}}
```
#### Girar a terceira página de um arquivo PDF em 90° no sentido horário, não modificando as restantes:
```shell
pdftk {{arquivo.pdf}} cat {{1-2 3east 4-end}} output {{novo_arquivo.pdf}}
```
{% endraw %}