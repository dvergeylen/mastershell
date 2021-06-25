---
layout: default
title: "bzip2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bzip2">
  <a href="/pt_br/common/bzip2.html">bzip2</a> <a href="#bzip2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um compressor de arquivos que utiliza o algoritmo Burrows–Wheeler.

#### Compactar um arquivo:
```shell
bzip2 {{arquivo}}
```
#### Descompactar um arquivo:
```shell
bzip2 -d {{arquivo.bz2}}
```
#### Descompactar um arquivo exibindo o conteúdo no terminal:
```shell
bzip2 -dc {{arquivo.bz2}}
```
{% endraw %}