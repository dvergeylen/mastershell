---
layout: default
title: "basename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="basename">
  <a href="/it/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restituisce la parte finale un percorso.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/basename>.

#### Mostra solo il nome del file da un percorso:
```shell
basename {{percorso/al/file}}
```
#### Mostra solo il nome di un file da un percorso, rimuovendo un suffisso:
```shell
basename {{percorso/al/file}} {{suffisso}}
```
{% endraw %}