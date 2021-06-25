---
layout: default
title: "man"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="man">
  <a href="/it/common/man.html">man</a> <a href="#man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Formatta e mostra pagine manuale.
> Maggiori informazioni: <https://www.man7.org/linux/man-pages/man1/man.1.html>.

#### Mostra la pagina di manuale di un comando:
```shell
man {{comando}}
```
#### Mostra la pagina di manuale per un comando dalla sezione 7:
```shell
man {{comando}}.{{7}}
```
#### Mostra il percorso in cui vengono cercate le pagine:
```shell
man --path
```
#### Mostra la posizione di una pagina invece che la pagina stessa:
```shell
man -w {{comando}}
```
#### Cerca pagine di manuale che contengano una certa stringa:
```shell
man -k {{ricerca}}
```
{% endraw %}