---
layout: default
title: "mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mv">
  <a href="/de/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verschiebe Dateien oder Verzeichnisse oder benenne diese um.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/mv>

#### Verschiebe eine Dateien an einen beliebigen Ort:
```shell
mv {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### Überschreibe bereits existierende Dateien ohne vorherige Bestätigung:
```shell
mv -f {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### Überschreibe bereits existierende Dateien nach Bestätigung (unabhängig von Dateirechten):
```shell
mv -i {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### Verhindere das Überschreiben existierender Dateien am Zielort:
```shell
mv -n {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
#### Liste Dateien und deren Details auf während sie verschoben werden:
```shell
mv -v {{pfad/zu/datei}} {{pfad/zu/zieldatei}}
```
{% endraw %}