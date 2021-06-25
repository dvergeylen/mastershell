---
layout: default
title: "calibredb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calibredb">
  <a href="/it/common/calibredb.html">calibredb</a> <a href="#calibredb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumentoi per gestire il tuo database di e-book.
> Parte del manager di e-book Calibre.
> Maggiori informazioni: <https://manual.calibre-ebook.com/generated/en/calibredb.html>.

#### Elenca gli e-book nella libreria con informazioni aggiuntive:
```shell
calibredb list
```
#### Cerca tra gli e-book mostrando informazioni aggiuntive:
```shell
calibredb list --search {{termine_di_ricerca}}
```
#### Cerca mostrando solamente gli ID degli e-book:
```shell
calibredb search {{termine_di_ricerca}}
```
#### Aggiungi uno o più e-book alla libreria:
```shell
calibredb add {{file1 file2 …}}
```
#### Rimuovi uno o più e-book dalla libreria. Sono necessari gli ID (vedi sopra):
```shell
calibredb remove {{id1 id2 …}}
```
{% endraw %}