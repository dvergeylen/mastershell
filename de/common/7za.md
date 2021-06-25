---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/de/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Dateiarchivierer mit hoher Kompressionsrate.
> Eine alleinstehende Version von `7z` mit Unterstützung für neuere Archivtypen.
> Weitere Informationen: <https://www.7-zip.org/>.

#### Archiviere eine Datei oder ein Verzeichnis:
```shell
7za a {{archiv.7z}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Extrahiere eine existierende 7z-Datei:
```shell
7za x {{archiv}}
```
#### Archiviere mit einem bestimmten Archivtyp:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{archiv}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Gib den Inhalt einer Archivdatei aus:
```shell
7za l {{archiv}}
```
#### Liste alle verfügbaren Archivtypen auf:
```shell
7za i
```
{% endraw %}