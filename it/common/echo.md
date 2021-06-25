---
layout: default
title: "echo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="echo">
  <a href="/it/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa a schermo gli argomenti forniti.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/echo>.

#### Stampa un messaggio di testo. Nota: le virgolette sono opzionali:
```shell
echo "{{Hello World}}"
```
#### Stampa un messaggio con il contenuto di variabili di ambiente:
```shell
echo "{{La mia path è $PATH}}"
```
#### Stampa un messaggio senza il carattere di nuova linea finale:
```shell
echo -n "{{Hello World}}"
```
#### Aggiungi un messaggio in coda ad un file:
```shell
echo "{{Hello World}}" >> {{file.txt}}
```
#### Abilita l'interpretazione delle sequenze di escape con il backslash (caratteri speciali):
```shell
echo -e "{{Colonna 1\tColonna 2}}"
```
{% endraw %}