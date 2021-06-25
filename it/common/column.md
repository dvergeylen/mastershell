---
layout: default
title: "column"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="column">
  <a href="/it/common/column.html">column</a> <a href="#column"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Formatta standard input o un file in più colonne.
> Le colonne sono riempite prima delle righe; il separatore predefinito è lo spazio.
> Maggiori informazioni: <https://manned.org/column>.

#### Formatta l'output per uno schermo largo 30 caratteri:
```shell
printf "intestazione1 intestazione2\nbar foo\n" | column --output-width {{30}}
```
#### Specifica un diverso separatore di colonna (e.g. "," per csv) (il predefinito è lo spazio):
```shell
printf "intestazione1 intestazione2\nbar foo\n" | column --separator {{,}}
```
#### Separa colonne ed allinea automaticamente in un formato tabulare:
```shell
printf "intestazione1 intestazione2\nbar foo\n" | column --table
```
#### Riempi le righe prima delle colonne:
```shell
printf "intestazione1\nbar\nfoobar\n" | column --output-width {{30}} --fillrows
```
{% endraw %}