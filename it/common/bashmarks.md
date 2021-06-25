---
layout: default
title: "bashmarks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bashmarks">
  <a href="/it/common/bashmarks.html">bashmarks</a> <a href="#bashmarks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Salva e salta a directory comunemente utilizzate usilizzando comandi di un carattere.
> Maggiori informazioni: <https://github.com/huyng/bashmarks>.

#### Elenca i segnalibri disponibili:
```shell
l
```
#### Salva la cartella corrente come segnalibro:
```shell
s {{nome_segnalibro}}
```
#### Vai ad una cartella salvata:
```shell
g {{nome_segnalibro}}
```
#### Lista i contenuti di una cartella salvata:
```shell
p {{nome_segnalibro}}
```
#### Elimina un segnalibro:
```shell
d {{nome_segnalibro}}
```
{% endraw %}