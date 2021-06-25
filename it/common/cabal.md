---
layout: default
title: "cabal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cabal">
  <a href="/it/common/cabal.html">cabal</a> <a href="#cabal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfaccia da linea di comando per l'infrastruttura di compilazione di Haskell (Cabal).
> Gestisce progetti Haskell e pacchetti Cabal dal repository di pacchetti Hackage.
> Maggiori informazioni: <https://cabal.readthedocs.io/en/latest/intro.html>.

#### Cerca ed elenca pacchetti da Hackage:
```shell
cabal list {{termine_di_ricerca}}
```
#### Mostra informazioni su di un pacchetto:
```shell
cabal info {{nome_pacchetto}}
```
#### Scarica ed installa un pacchetto:
```shell
cabal install {{nome_pacchetto}}
```
#### Crea un nuovo progetto Haskell nella directory corrente:
```shell
cabal init
```
#### Compila il progetto nella directory corrente:
```shell
cabal build
```
#### Esegui i test del progetto nella directory corrente:
```shell
cabal test
```
{% endraw %}