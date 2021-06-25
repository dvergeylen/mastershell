---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/de/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Dateiarchivierer mit hoher Kompressionsrate.
> Eine alleinstehende Version von `7z`, die nur .7z Dateien unterstützt.
> Weitere Informationen: <https://www.7-zip.org/>.

#### Archiviere eine Datei oder ein Verzeichnis:
```shell
7zr a {{archiv.7z}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Extrahiere eine existierende 7z-Datei:
```shell
7zr x {{archiv.7z}}
```
#### Gib den Inhalt einer Archivdatei aus:
```shell
7zr l {{archiv}}
```
{% endraw %}