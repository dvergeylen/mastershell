---
layout: default
title: "xz"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xz">
  <a href="/pt_br/common/xz.html">xz</a> <a href="#xz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compactar ou descompactar arquivos com a extensão .xz ou .lzma.
> Mais informações: <https://tukaani.org/xz/format.html>.

#### Compactar um arquivo no formato xz:
```shell
xz {{arquivo}}
```
#### Descompactar um arquivo no formato xz:
```shell
xz -d {{arquivo.xz}}
```
#### Compactar um arquivo no formato lzma:
```shell
xz --format=lzma {{arquivo}}
```
#### Descompactar um arquivo no formato lzma:
```shell
xz -d --format=lzma {{arquivo.lzma}}
```
#### Descompactar um arquivo e escrever a saída no terminal:
```shell
xz -dc {{arquivo.xz}}
```
#### Compactar um arquivo sem apagar o arquivo original:
```shell
xz -k {{arquivo}}
```
#### Compactar um arquivo utilizando a compactação mais rápida:
```shell
xz -0 {{arquivo}}
```
#### Compactar um arquivo utilizando a compactação mais eficiente:
```shell
xz -9 {{arquivo}}
```
{% endraw %}