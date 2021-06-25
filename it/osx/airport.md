---
layout: default
title: "airport"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airport">
  <a href="/it/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di configurazione delle reti senza fili.

#### Mostra le informazioni relative allo stato attuale delle connessioni senza fili:
```shell
airport -I
```
#### Intercetta il traffico delle connessioni senza fili sul primo canale:
```shell
airport sniff {{1}}
```
#### Ricerca le reti senza fili disponibili:
```shell
airport -s
```
#### Disassocia dalla rete airport corrente:
```shell
sudo airport -z
```
{% endraw %}