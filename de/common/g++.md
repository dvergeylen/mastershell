---
layout: default
title: "gplusplus"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gplusplus">
  <a href="/de/common/g++.html">gplusplus</a> <a href="#gplusplus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere C++ Quelldateien.
> Teil der GCC (GNU Compiler Collection).
> Weitere Informationen: <https://gcc.gnu.org>.

#### Kompiliere eine Quelldatei in eine ausführbare Binärdatei:
```shell
g++ {{quelldatei.cpp}} -o {{output_datei}}
```
#### Zeige (fast) alle Fehler und Warnungen an:
```shell
g++ {{quelldatei.cpp}} -Wall -o {{output_datei}}
```
#### Wähle einen Sprachstandard für das Kompilieren:
```shell
g++ {{quelldatei.cpp}} -std={{C++98|C++11|C++14|C++17}} -o {{output_datei}}
```
#### Binde Bibliotheken, die sich an einem anderen Pfad als die Quelldatei befinden mit ein:
```shell
g++ {{quelldatei.cpp}} -o {{output_datei}} -I{{header_pfad}} -L{{bibliotheks_pfad}} -l{{bibliotheks_name}}
```
{% endraw %}