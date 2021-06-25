---
layout: default
title: "cut"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cut">
  <a href="/it/common/cut.html">cut</a> <a href="#cut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Taglia dividendo in campi stdin o file.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/cut>.

#### Estrai i primi 16 caratteri di ogni riga da stdin:
```shell
cut -c {{1-16}}
```
#### Estrai i primi 16 caratteri di ogni riga da un dato file:
```shell
cut -c {{1-16}} {{file}}
```
#### Estrai tutto dal terzo carattere fino alla fine di ogni riga:
```shell
cut -c {{3-}}
```
#### Estrai il quinto campo di ogni linea, utilizzando i due punti come separatore di campo (il default è tab):
```shell
cut -d'{{:}}' -f{{5}}
```
#### Estrai il secondo e decimo campo di ogni linea, utilizzando il punto e virgola come delimitatore:
```shell
cut -d'{{;}}' -f{{2,10}}
```
#### Estrai i campi dal terzo in poi di ogni linea, utilizzando lo spazio come delimitatore:
```shell
cut -d'{{ }}' -f{{3-}}
```
{% endraw %}