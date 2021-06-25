---
layout: default
title: "cmake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmake">
  <a href="/it/common/cmake.html">cmake</a> <a href="#cmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generatore di ambienti di compilazione multipiattaforma.
> Genera Makefile, progetti Visual Studio o altro, in base al sistema operativo.
> Maggiori informazioni: <https://cmake.org/cmake/help/v3.2/manual/cmake.1.html>.

#### Genera un Makefile ed usalo per compilare un progetto nella stessa directory dei sorgenti:
```shell
cmake && make
```
#### Genera un makefile ed usalo per compilare un progetto in una directory "build" separata (out-of-source build):
```shell
cmake -H. -B{{build}} && make -C {{build}}
```
#### Esegui cmake in modalità interattiva (chiederà i valori di ogni variabile invece di usare i predefiniti):
```shell
cmake -i
```
{% endraw %}