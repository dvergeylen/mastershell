---
layout: default
title: "unrar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unrar">
  <a href="/pt_br/common/unrar.html">unrar</a> <a href="#unrar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Descompactar arquivos comprimidos no formato RAR.

#### Descompactar o arquivo mantendo a estrutura de diretórios original:
```shell
unrar x {{arquivo.rar}}
```
#### Descompactar o arquivo sem manter a estrutura de diretórios original:
```shell
unrar e {{arquivo.rar}}
```
#### Verificar a integridade do conteúdo de um arquivo:
```shell
unrar t {{arquivo.rar}}
```
#### Exibir o conteúdo de um arquivo sem descompactá-lo:
```shell
unrar l {{arquivo.rar}}
```
{% endraw %}