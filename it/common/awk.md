---
layout: default
title: "awk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="awk">
  <a href="/it/common/awk.html">awk</a> <a href="#awk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un versatile linguaggio di programmazione per elaborare file.
> Maggiori informazioni: <https://github.com/onetrueawk/awk>.

#### Stampa la quinta colonna (field) in un file di linee separate da spazi:
```shell
awk '{print $5}' {{nome_file}}
```
#### Stampa la seconda colonna delle linee contenenti "qualcosa":
```shell
awk '/{{qualcosa}}/ {print $2}' {{nome_file}}
```
#### Stampa l'ultima colonna di ogni linea di un file, utilizzando la virgola (invece dello spazio) come separatore di colonne:
```shell
awk -F ',' '{print $NF}' {{nome_file}}
```
#### Somma i valori nella prima colonna di un file e stampa il totale:
```shell
awk '{s+=$1} END {print s}' {{nome_file}}
```
#### Somma i valori nella prima colonna e stampali seguiti dal totale:
```shell
awk '{s+=$1; print $1} END {print "--------"; print s}' {{nome_file}}
```
#### Stampa una liena ogni tre iniziando dalla prima:
```shell
awk 'NR%3==1' {{nome_file}}
```
{% endraw %}