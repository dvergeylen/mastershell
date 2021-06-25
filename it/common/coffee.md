---
layout: default
title: "coffee"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="coffee">
  <a href="/it/common/coffee.html">coffee</a> <a href="#coffee"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui script CoffeScript o compilali in JavaScript.
> Maggiori informazioni: <https://coffeescript.org#cli>.

#### Esegui uno script:
```shell
coffee {{percorso/al/file.coffee}}
```
#### Compila in JavaScript e salva lo script con lo stesso nome:
```shell
coffee --compile {{percorso/al/file.coffee}}
```
#### Compila in JavaScript e salva lo script specificandone il nome:
```shell
coffee --compile {{percorso/al/file.coffee}} --output {{percorso/al/file.js}}
```
#### Esegui una console REPL interattiva:
```shell
coffee --interactive
```
#### Monitora cambiamenti in uno script rieseguendolo ogni volta:
```shell
coffee --watch {{percorso/al/file.coffee}}
```
{% endraw %}