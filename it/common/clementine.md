---
layout: default
title: "clementine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clementine">
  <a href="/it/common/clementine.html">clementine</a> <a href="#clementine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un moderno player e gestore di librerie musicali.
> Maggiori informazioni: <https://www.clementine-player.org>.

#### Apri Clementine:
```shell
clementine
```
#### Avvia la riproduzione di un file musicale:
```shell
clementine {{URL|percorso/a/file}}
```
#### Pausa o riprendi la riproduzione:
```shell
clementine --play-pause
```
#### Ferma la riproduzione:
```shell
clementine --stop
```
#### Passa alla prossima traccia:
```shell
clementine --next
```
#### Passa alla traccia precedente:
```shell
clementine --previous
```
#### Carica un file playlist:
```shell
clementine --load {{percorso/a/file_playlist}}
```
#### Riproduci la quinta traccia nella playlist attualmente caricata:
```shell
clementine --play-track {{5}}
```
{% endraw %}