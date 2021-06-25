---
layout: default
title: "dpkg-query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg-query">
  <a href="/it/linux/dpkg-query.html">dpkg-query</a> <a href="#dpkg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uno strumento che mostra informazioni sui pacchetti installati.

#### Elenca tutti i pacchetti installati:
```shell
dpkg-query -l
```
#### Elenca i pacchetti installati con nomi che combaciano con una data espressione:
```shell
dpkg-query -l '{{espressione_pattern}}'
```
#### Elenca tutti i file installati da una pacchetto:
```shell
dpkg-query -L {{nome_del_pacchetto}}
```
#### Mostra le informazioni riguardanti un pacchetto:
```shell
dpkg-query -s {{nome_del_pacchetto}}
```
{% endraw %}