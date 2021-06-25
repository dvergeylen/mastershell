---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/de/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verkette und gib einzelne oder mehrere Dateien aus.
> Mehrere Informationen: <https://www.gnu.org/software/coreutils/cat>.

#### Gib den Inhalt einer Datei aus:
```shell
cat {{pfad/zu/datei}}
```
#### Verkette mehrere Dateien und speichere das Ergebnis in einer neuen Datei:
```shell
cat {{pfad/zu/datei1}} {{pfad/zu/datei2}} > {{pfad/zu/ziel_datei}}
```
#### Verkette mehrere Dateien und hänge des Ergebnis an eine Datei an:
```shell
cat {{pfad/zu/datei1}} {{pfad/zu/datei2}} >> {{pfad/zu/ziel_datei}}
```
#### Nummeriere alle ausgegebenen Zeilen:
```shell
cat -n {{pfad/zu/datei}}
```
#### Gib eine Datei inklusive aller unsichtbaren Leerzeichen aus (mit `M-` Präfix wenn sie nicht ASCII sind):
```shell
cat -v -t -e {{pfad/zu/datei}}
```
{% endraw %}