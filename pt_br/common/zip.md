---
layout: default
title: "zip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zip">
  <a href="/pt_br/common/zip.html">zip</a> <a href="#zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de compressão de arquivos em arquivos zip.

#### Compactando arquivos em um arquivo zip:
```shell
zip {{output.zip}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Compactando todos os arquivos de um diretório:
```shell
zip {{output.zip}} {{caminho/do/diretorio/*}}
```
#### Adicionando arquivos a um arquivo zip existente:
```shell
zip {{arquivo_existente.zip}} {{caminho/do/diretorio}}
```
#### Compactando todos os arquivos de um diretório mantendo estruturas de diretórios:
```shell
zip -r {{output.zip}} {{caminho/do/diretorio}}
```
#### Compactando arquivos de um diretório excluindo arquivos específicos:
```shell
zip -r {{output.zip}} {{caminho/do/diretorio}} -x {{caminho/a/ser/excluido}}
```
#### Compactando arquivos definindo o nível de compressão [9]:
```shell
zip -r -{{9}} {{output.zip}} {{caminho/do/diretorio}}
```
#### Deletando arquivos de um arquivo zip:
```shell
zip -d {{output.zip}} "{{foo/*.ext}}"
```
{% endraw %}