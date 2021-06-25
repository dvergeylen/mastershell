---
layout: default
title: "bc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bc">
  <a href="/it/common/bc.html">bc</a> <a href="#bc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calcolatore.
> Maggiori informazioni: <https://manned.org/bc>.

#### Esegui in modalità interattiva utilizzando la libreria math della standard library:
```shell
bc -l
```
#### Calcola il risultato di un'espressione:
```shell
bc <<< "(1 + 2) * 2 ^ 2"
```
#### Calcola un'espressione forzando il numero di decimali usati a 10:
```shell
bc <<< "scale=10; 5 / 3"
```
#### Calcola un'espressione con seno e coseno utilizzando mathlib:
```shell
bc -l <<< "s(1) + c(1)"
```
{% endraw %}