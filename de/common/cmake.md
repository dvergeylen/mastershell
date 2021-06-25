---
layout: default
title: "cmake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmake">
  <a href="/de/common/cmake.html">cmake</a> <a href="#cmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plattformübergreifndes Build-Automatisierungs-System, das Vorlagen für native Build-Systeme erzeugt.
> Weitere Informationen: <https://cmake.org/cmake/help/latest/manual/cmake.1.html>.

#### Erzeuge eine Build-Vorlage im aktuellen Verzeichnis mit `CMakeLists.txt` eines Projektordners:
```shell
cmake {{pfad/zu/projektordner}}
```
#### Erzeuge eine Build-Vorlage mit der Build-Art `Release`:
```shell
cmake {{pfad/zu/projektordner}} -D {{CMAKE_BUILD_TYPE=Release}}
```
#### Benutze eine generierte Vorlage, um Artifakte zu erzeugen:
```shell
cmake --build {{pfad/zu/build_verzeichnis}}
```
#### Installiere die Build-Artifakte in `/usr/local/` und enferne Debugsymbole:
```shell
cmake --install {{pfad/zu/build_verzeichnis}} --strip
```
#### Installiere die Build-Artifakte mit einem eigenen Präfix für Pfade:
```shell
cmake --install {{pfad/zu/build_verzeichnis}} --strip --prefix {{pfad/zu/verzeichnis}}
```
#### Führe ein bestimmtes Build-Ziel aus:
```shell
cmake --build {{pfad/zu/build_verzeichnis}} --target {{zielname}}
```
{% endraw %}