---
layout: default
title: "autoflake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autoflake">
  <a href="/it/common/autoflake.html">autoflake</a> <a href="#autoflake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uno strumento per rimuovere import e variabili inutilizzati da codice Python.
> Maggiori informazioni: <https://github.com/myint/autoflake>.

#### Rimuovi le variabili inutilizzate da un file e mostra la differenza:
```shell
autoflake --remove-unused-variables {{file.py}}
```
#### Rimuovi gli import inutilizzati da multipli file mostrando le differenze:
```shell
autoflake --remove-all-unused-imports {{file1.py}} {{file2.py}} {{file3.py}}
```
#### Rimuovi le variabili inutilizzate da un file, sovrascrivendolo:
```shell
autoflake --remove-unused-variables --in-place {{file.py}}
```
#### Rimuovi le variabili inutilizzate da tutti i file in una cartella, ricorsivamente e sovrascrivendoli:
```shell
autoflake --remove-unused-variables --in-place --recursive {{percorso/a/cartella}}
```
{% endraw %}