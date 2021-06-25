---
layout: default
title: "ed"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ed">
  <a href="/it/common/ed.html">ed</a> <a href="#ed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> L'originale editor di testo Unix.
> Maggiori informazioni: <https://man.archlinux.org/man/ed.1>.

#### Avvia ed per editare un documento vuoto (che può essere salvato come nuovo file nella directory corrente):
```shell
ed
```
#### Avvia ed per editare un documento vuoto, con `:` come indicatore del prompt di comandi:
```shell
ed -p :
```
#### Avvia ed per editare un file esistente (mostra il numero di byte del file caricato):
```shell
ed -p : {{percorso/al/file}}
```
#### Attiva o disattiva la stampa di spiegazioni per gli errori (di default, le spiegazioni non sono stampate ed appare solo un `?`):
```shell
H
```
#### Aggiungi del testo al documento corrente. Indica il completamento inserendo un punto da solo su una nuova linea:
```shell
a<Enter>{{text_to_insert}}<Enter>.
```
#### Stampa l'intero documento (`,` è una scorciatoia per il range `1,$` che copre dall'inizio alla fine del documento):
```shell
,p
```
#### Scrivi il documento corrente su un nuovo file (il nome del file può essere omesso se `ed` è stato avviato con un file esistente):
```shell
w {{nome_file}}
```
#### Termina ed:
```shell
q
```
{% endraw %}