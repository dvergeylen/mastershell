---
layout: default
title: "less"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="less">
  <a href="/it/common/less.html">less</a> <a href="#less"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apri un file per lettura interattiva, permettendo di scorrere e cercare testo al suo interno.

#### Apri un file:
```shell
less {{file}}
```
#### Muoviti una pagina in giù / su:
```shell
<Spazio> (giù), b (su)
```
#### Vai alla fine o all'inizio del file:
```shell
G (fine), g (inizio)
```
#### Cerca una stringa in avanti (usa `n`/`N` per muoverti al risultato successivo/precedente):
```shell
/{{stinga}}
```
#### Cerca una stringa indietro (usa `n`/`N` per muoverti al risultato successivo/precedente):
```shell
?{{stringa}}
```
#### Aggiorna il file dinamicamente:
```shell
F
```
#### Apri il file in un editor di testo:
```shell
v
```
#### Esci:
```shell
q
```
{% endraw %}