---
layout: default
title: "caffeinate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="caffeinate">
  <a href="/it/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Impedisci al mac di sospendersi.

#### Impedisci la sospensione per un'ora (3600 secondi):
```shell
caffeinate -u -t {{3600}}
```
#### Impedisci la sospensione fino al completamento dell'esecuzione di un comando:
```shell
caffeinate -s {{comando}}
```
#### Impedisci la sospensione fino alla pressione della combinazione di tasti Ctrl-C:
```shell
caffeinate -i
```
{% endraw %}