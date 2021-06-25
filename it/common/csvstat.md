---
layout: default
title: "csvstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvstat">
  <a href="/it/common/csvstat.html">csvstat</a> <a href="#csvstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa statistiche descrittive per tutte le colonne di un file CSV.
> Incluso in csvkit.
> Maggiori informazioni: <https://csvkit.readthedocs.io/en/latest/scripts/csvstat.html>.

#### Mostra tutte le statistiche per tutte le colonne:
```shell
csvstat {{dati.csv}}
```
#### Mostra tutte le statistiche per le colonne 2 e 4:
```shell
csvstat -c {{2,4}} {{dati.csv}}
```
#### Mostra la somma per tutte le colonne:
```shell
csvstat --sum {{dati.csv}}
```
#### Mostra la lunghezza massima dei valori della colonna 3:
```shell
csvstat -c {{3}} --len {{dati.csv}}
```
#### Mostra il numedo di valori unici nella colonna "nome":
```shell
csvstat -c {{nome}} --unique {{dati.csv}}
```
{% endraw %}