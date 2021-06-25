---
layout: default
title: "banner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="banner">
  <a href="/it/common/banner.html">banner</a> <a href="#banner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa il testo fornito per argomento come un grande banner in ASCII art.
> Maggiori informazioni: <https://man.archlinux.org/man/banner.1>.

#### Stampa il testo come un grande banner (le virgolette sono opzionali):
```shell
banner "{{Hello World}}"
```
#### Stampa il testo come un banner con una larghezza di 50 caratteri:
```shell
banner -w {{50}} "{{Hello World}}"
```
#### Leggi testo da stdin:
```shell
banner
```
{% endraw %}