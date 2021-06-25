---
layout: default
title: "unzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unzip">
  <a href="/pt_br/common/unzip.html">unzip</a> <a href="#unzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de descompactação de arquivos zip.

#### Extraindo arquivos zip:
```shell
unzip {{arquivo.zip}}
```
#### Extraindo arquivos zip para caminhos específicos:
```shell
unzip {{arquivo.zip}} -d {{caminho/para}}
```
#### Listando conteúdos de arquivos zip:
```shell
unzip -l {{arquivo.zip}}
```
#### Extraindo arquivos zip sobrescrevendo outros arquivos:
```shell
unzip -o {{arquivo.zip}}
```
#### Extraindo arquivos zip não sobrescrevendo outros arquivos:
```shell
unzip -n {{arquivo.zip}}
```
#### Extraindo arquivos zip sem a estrutura dos diretórios:
```shell
unzip -j {{arquivo.zip}}
```
{% endraw %}