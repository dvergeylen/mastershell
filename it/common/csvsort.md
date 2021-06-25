---
layout: default
title: "csvsort"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvsort">
  <a href="/it/common/csvsort.html">csvsort</a> <a href="#csvsort"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ordina le righe di di file CSV.
> Incluso in csvkit.
> Maggiori informazioni: <https://csvkit.readthedocs.io/en/latest/scripts/csvsort.html>.

#### Ordina un file CSV secondo la colonna 9:
```shell
csvsort -c {{9}} {{data.csv}}
```
#### Ordina un file CSV secondo la colonna "nome" in ordine decrescente:
```shell
csvsort -r -c {{nome}} {{data.csv}}
```
#### Ordina un file CSV secondo la colonna 2 e secondo la 4:
```shell
csvsort -c {{2,4}} {{data.csv}}
```
#### Ordina un file CSV senza inferire il tipo dei dati:
```shell
csvsort --no-inference -c {{colonne}} {{data.csv}}
```
{% endraw %}