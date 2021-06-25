---
layout: default
title: "dirname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirname">
  <a href="/it/common/dirname.html">dirname</a> <a href="#dirname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Determina la directory genitore di un determinato file o percorso.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/dirname>.

#### Calcola la directory genitore di un dato percorso:
```shell
dirname {{percorso/a/file_o_directory}}
```
#### Calcola la directory genitore di più percorsi:
```shell
dirname {{percorso/a/file_a}} {{percorso/a/directory_b}}
```
#### Delimita l'output con caratteri NUL invece di newline (utile in combinazione con `xargs`):
```shell
dirname --zero {{percorso/a/directory_a}} {{percorso/a/file_b}}
```
{% endraw %}