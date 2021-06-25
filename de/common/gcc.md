---
layout: default
title: "gcc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gcc">
  <a href="/de/common/gcc.html">gcc</a> <a href="#gcc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Präprozessiert und kompiliert C und C++ Quellcodedateien und linkt diese anschließend zusammen.
> Weitere Informationen: <https://gcc.gnu.org>.

#### Kompiliere mehrere Quellcodedateien zu einer ausführbaren Datei:
```shell
gcc {{pfad/zu/datei1.c}} {{pfad/zu/datei2.c}} -o {{pfad/zu/binärdatei}}
```
#### Erlaube Warnungen und debug-Symbole in der Ausgabedatei:
```shell
gcc {{pfad/zu/datei.c}} -Wall -Og -o {{pfad/zu/binärdatei}}
```
#### Inkludiere Bibliotheken aus anderen Verzeichnissen:
```shell
gcc {{pfad/zu/datei.c}} -o {{pfad/zu/binärdatei}} -I{{pfad/zu/headerdatei}} -L{{pfad/zu/bibliothek1}} -l{{pfad/zu/bibliothek2}}
```
#### Kompiliere Quellcodedateien zu Assemblerinstruktionen:
```shell
gcc -S {{pfad/zu/datei.c}}
```
#### Kompiliere eine oder mehrere Quellcodedateien ohne diese zu linken:
```shell
gcc -c {{pfad/zu/datei.c}}
```
{% endraw %}