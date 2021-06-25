---
layout: default
title: "box"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="box">
  <a href="/it/common/box.html">box</a> <a href="#box"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Una applicazione PHP per creare e gestire Phars.
> Maggiori informazioni: <https://box-project.github.io/box2>.

#### Crea un nuovo file Phar:
```shell
box build
```
#### Crea un nuovo file Phar usando uno specifico file di configurazione:
```shell
box build -c {{percorso/a/configurazione}}
```
#### Mostra informazioni sulla estensione PHP PHAR:
```shell
box info
```
#### Mostra informazioni su di uno specifico file Phar:
```shell
box info {{percorso/a/file_phar}}
```
#### Valida il primo file di configurazione trovato nella directory corrente:
```shell
box validate
```
#### Verifica la firma di uno specifico file Phar:
```shell
box verify {{percorso/a/file_phar}}
```
#### Mostra tutti i comandi ed opzioni disponibili:
```shell
box help
```
{% endraw %}