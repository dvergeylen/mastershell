---
layout: default
title: "babel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="babel">
  <a href="/it/common/babel.html">babel</a> <a href="#babel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un transpiler che converte codice JavaScript da sintassi ES6/ES7 ad ES5.
> Maggiori informazioni: <https://babeljs.io/>.

#### Transpila uno specifico file e stampa il risultato su stdout:
```shell
babel {{percorso/al/file}}
```
#### Transpila un file e scrivi il risultato su uno specifico file di output:
```shell
babel {{percorso/al/file_input}} --out-file {{percorso/al/file_output}}
```
#### Transpila un file ogni volta che viene modificato:
```shell
babel {{percorso/al/file}} --watch
```
#### Transpila un'intera directory di file:
```shell
babel {{percorso/a/directory_input}}
```
#### Transpila un'intera directory ignorando specifici file separati da virgola:
```shell
babel {{percorso/a/directory_input}} --ignore {{file_ignorati}}
```
#### Transpila minimizzando il codice JavaScript in output:
```shell
babel {{percorso/al/file_input}} --minified
```
#### Scegli un insieme di preset per formattare l'output:
```shell
babel {{percorso/al/file_input}} --presets {{preset}}
```
#### Mostra tutte le opzioni disponibili:
```shell
babel --help
```
{% endraw %}