---
layout: default
title: "head"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="head">
  <a href="/it/common/head.html">head</a> <a href="#head"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa a schermo le prime linee di un file.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/head>.

#### Stampa a schermo le prime linee di un file:
```shell
head -n {{numero_di_linee}} {{file}}
```
#### Stampa a schermo i primi byte di un file:
```shell
head -c {{numero_di_byte}} {{file}}
```
#### Stampa a schermo tutto il file meno le ultime linee:
```shell
head -n -{{numero_di_linee}} {{file}}
```
#### Stampa a schermo tutto il file meno gli ultimi byte:
```shell
head -c -{{numero_di_byte}} {{file}}
```
{% endraw %}