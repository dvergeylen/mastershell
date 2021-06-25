---
layout: default
title: "du"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="du">
  <a href="/it/common/du.html">du</a> <a href="#du"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilizzo del disco: stima e riassumi lo spazio utilizzato da file e directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/du>.

#### Elenca le dimensioni di una directory ed ogni sotto-directory, nell'unità specificata (B/KB/MB):
```shell
du -{{b|k|m}} {{percorso/alla/directory}}
```
#### Elenca le dimensioni di una directory ed ogni sotto-directory, in formato umanamente leggibile (seleziona automaticamente l'unità appropriata per ogni dimensione):
```shell
du -h {{percorso/alla/directory}}
```
#### Mostra la dimensione di una singola directory, in unità umanamente leggibili:
```shell
du -sh {{percorso/alla/directory}}
```
#### Mostra in formato umanamente leggibile le dimensioni di una directory e tutti i file e directory in essa contenuti:
```shell
du -ah {{percorso/alla/directory}}
```
#### Elenca le dimensioni umanamente leggibili di una directory e d ogni sotto-directory, fino ad N livelli di profondità:
```shell
du -h --max-depth=N {{percorso/alla/directory}}
```
#### Mostra le dimensioni umanamente leggibili di tutti i file `.jpg` nelle sottocartelle della cartella corrente, e mostra il totale cumulativo alla fine:
```shell
du -ch */*.jpg
```
{% endraw %}