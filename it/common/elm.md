---
layout: default
title: "elm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="elm">
  <a href="/it/common/elm.html">elm</a> <a href="#elm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compila ed esegui file sorgente Elm.
> Maggiori informazioni: <https://elm-lang.org>.

#### Inizializza un progetto Elm, generando un file `elm.json`:
```shell
elm init
```
#### Avvia una shell Elm interattiva:
```shell
elm repl
```
#### Compila un file Elm, scrivendo il risultato in un file `index.html`:
```shell
elm make {{sorgente}}
```
#### Compila un file Elm, scrivendo il risultato in un file JavaScript:
```shell
elm make {{sorgente}} --output={{destinazione}}.js
```
#### Avvia un web server locale che compila file Elm al caricamento delle pagine:
```shell
elm reactor
```
#### Installa un pacchetto Elm da https://package.elm-lang.org:
```shell
elm install {{author}}/{{package}}
```
{% endraw %}