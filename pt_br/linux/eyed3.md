---
layout: default
title: "eyeD3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eyed3">
  <a href="/pt_br/linux/eyed3.html">eyeD3</a> <a href="#eyed3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lê e manipula os metadados de arquivos MP3.
> Mais informações: <https://eyed3.readthedocs.io/en/latest/>.

#### Visualizar as informações de um arquivo MP3:
```shell
eyeD3 {{arquivo.mp3}}
```
#### Definir o título de um arquivo MP3:
```shell
eyeD3 --title "{{titulo}}" {{arquivo.mp3}}
```
#### Definir o álbum de todos os arquivos MP3 de um diretório:
```shell
eyeD3 --album "{{nome_do_album}}" {{*.mp3}}
```
#### Definir a capa do álbum para um arquivo MP3:
```shell
eyeD3 --add-image {{capa.jpeg}}:FRONT_COVER: {{arquivo.mp3}}
```
{% endraw %}