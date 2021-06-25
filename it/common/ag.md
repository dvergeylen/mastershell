---
layout: default
title: "ag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ag">
  <a href="/it/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. Come `ack`, ma più veloce.
> Maggiori informazioni: <https://github.com/ggreer/the_silver_searcher>.

#### Trova file contenenti "foo" e mostra le corrisponenti linee contenenti il termine:
```shell
ag {{foo}}
```
#### Trova file contenenti "foo" in una specifica directory:
```shell
ag {{foo}} {{percorso/alla/directory}}
```
#### Trova file contenenti "foo" elencandone solamente i nomi:
```shell
ag -l {{foo}}
```
#### Trova file contenenti "FOO" senza distinguere tra maiuscole e minuscole, e stampa solo il termine trovato piuttosto che l'intera linea:
```shell
ag -i -o {{FOO}}
```
#### Trova "foo" in file il quale nome contiene "bar":
```shell
ag {{foo}} -G {{bar}}
```
#### Trova file il quale contenuto soddisfi una determinata espressione regolare:
```shell
ag '{{espressione_regolare}}'
```
#### Trova file il quale nome contiene "foo":
```shell
ag -g {{foo}}
```
{% endraw %}