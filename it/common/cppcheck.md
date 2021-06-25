---
layout: default
title: "cppcheck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cppcheck">
  <a href="/it/common/cppcheck.html">cppcheck</a> <a href="#cppcheck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di analisi statica per codice C/C++.
> Piuttosto che sugli errori di sintassi, si concentra su tipi di bug che normalmente non vengono rilevati dai compilatori.
> Maggiori informazioni: <http://cppcheck.sourceforge.net>.

#### Controlla la directory corrente ricorsivamente, mostrando il progresso a schermo e loggando i messaggi di errore in un file:
```shell
cppcheck . 2> cppcheck.log
```
#### Controlla una determinata directory ricorsivamente, senza stampare informazioni sul progresso:
```shell
cppcheck --quiet {{path/to/directory}}
```
#### Controlla un determinato file, specificando quali test eseguire (di default, solo gli errori sono mostrati):
```shell
cppcheck --enable={{error|warning|style|performance|portability|information|all}} {{percorso/al/file.cpp}}
```
#### Elenca i test disponibili:
```shell
cppcheck --errorlist
```
#### Controlla un determinato file, ignorando specifici test:
```shell
cppcheck --suppress={{id_test1}} --suppress={{it_test2}} {{percorso/al/file.cpp}}
```
#### Controlla la directory corrente, fornendo percorsi da includere per file esterni (e.g. librerie esterne):
```shell
cppcheck -I {{include/directory_1}} -I {{include/directory_2}} .
```
#### Controlla un progetto Microsoft Visual Studio (`*.vcxproj`) o file solution (`*.sln`):
```shell
cppcheck --project={{path/to/progetto.sln}}
```
{% endraw %}