---
layout: default
title: "elinks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="elinks">
  <a href="/it/common/elinks.html">elinks</a> <a href="#elinks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un browser testuale simile a lynx.
> Maggiori informazioni: <http://elinks.or.cz>.

#### Avvia elinks:
```shell
elinks
```
#### Termina elinks:
```shell
Ctrl + C
```
#### Stampa l'output di una pagina web nella console, colorando il testo con codici di controllo ANSI:
```shell
elinks -dump -dump-color-mode {{1}} {{url}}
```
{% endraw %}