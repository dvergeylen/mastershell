---
layout: default
title: "dc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dc">
  <a href="/it/common/dc.html">dc</a> <a href="#dc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calcolatore a precisione arbitraria. Usa la notazione polacca inversa (RPN).
> Maggiori informazioni: <https://www.gnu.org/software/bc/manual/dc-1.05/html_mono/dc.html>.

#### Avvia il calcolatore in modalità interattiva:
```shell
dc
```
#### Esegui uno script dc da file:
```shell
dc -f {{file}}
```
#### Calcola 4 per 5 [4 5 *], sottrai 17 [17 -], e stampa [p] il risultato (utilizzando echo):
```shell
echo "4 5 * 17 - p"| dc
```
#### Setta il numero di posizioni decimali a 7 [7 k], calcola 5 diviso -3 [5 _3/] e stampa [p] il risultato (utilizzando dc -e):
```shell
dc -e "7 k 5 _3 / p"
```
#### Calcola il rapporto aureo, phi: setta il numero di posizioni decimali a 100 [100 k], e calcola la radice di 5 [5 v] più 1 [1 +], diviso due [2 /] e stampa [p] il risultato:
```shell
dc -e "100 k 5 v 1 + 2 / p"
```
{% endraw %}