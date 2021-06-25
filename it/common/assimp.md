---
layout: default
title: "assimp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="assimp">
  <a href="/it/common/assimp.html">assimp</a> <a href="#assimp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Client da linea di comando per la Open Asset Import Library.
> Supporta il caricamento di 40+ formati di file per modelli 3D, e l'espoerazione di diversi formati 3D popolari.
> Maggiori informazioni: <http://www.assimp.org/>.

#### Elenca tutti i formati supportati:
```shell
assimp listext
```
#### Elenca tutti i formati supportati per l'esportazione:
```shell
assimp listexport
```
#### Converti un file a uno dei tipi supportati, utilizzando i parametri predefiniti:
```shell
assimp export {{file_input.stl}} {{file_output.obj}}
```
#### Converti un file utilizzando parametri personalizzati (il file dox_cmd.h nel source code di assimp contiene una lista di parametri disponibili):
```shell
assimp export {{file_input.stl}} {{file_output.obj}} {{parametri}}
```
#### Mostra un riepilogo del contenuto di un file:
```shell
assimp info {{percordo/al/file}}
```
#### Elenca tutti i sottocomandi disponibili (detti "verbs"):
```shell
assimp help
```
#### Chiedi aiuto per uno specifico sottocomando (ad esempio riguardo i suoi parametri):
```shell
assimp {{sottocomando}} --help
```
{% endraw %}