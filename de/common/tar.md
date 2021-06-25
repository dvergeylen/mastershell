---
layout: default
title: "tar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tar">
  <a href="/de/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archivierungs Tool.
> Häufig kombiniert mit anderen Methoden zur Komprimierung, wie gzip oder bzip2.
> Weitere Informationen: <https://www.gnu.org/software/tar>.

#### Erstelle ein Archiv von Datein:
```shell
tar cf {{pfad/zu/ziel.tar}} {{pfad/zu/datei1}} {{pfad/zu/datei2}} {{pfad/zu/datei3}}
```
#### Erstelle ein mit gzip komprimiertes Archiv:
```shell
tar czf {{ziel.tar.gz}} {{pfad/zu/datei1}} {{pfad/zu/datei2}} {{pfad/zu/datei3}}
```
#### Erstelle ein mit gzip komprimiertes Archiv mit relativen Pfaden:
```shell
tar czf {{pfad/zu/ziel.tar.gz}} -C {{pfad/zu/verzeichniss/}} .
```
#### Extrahiere ein (komprimiertes) Archiv in das derzeitige Verzeichniss:
```shell
tar xf {{pfad/zu/quelle.tar[.gz|.bz2|.xz]}}
```
#### Extrahiere ein Archiv in ein Verzeichniss:
```shell
tar xf {{pfad/zu/quelle.tar}} -C {{verzeichniss}}
```
#### Erstelle ein komprimiertes Archiv und benutze den Archiv Suffix um die Kompressionsmethode zu wählen:
```shell
tar caf {{ziel.tar.xz}} {{pfad/zu/datei1}} {{pfad/zu/datei2}} {{pfad/zu/datei3}}
```
#### Führe die Inhalte eines tar Archivs auf:
```shell
tar tvf {{pfad/zu/quelle.tar}}
```
#### Extrahiere Dateien die mit einem Muster übereinstimmen:
```shell
tar xf {{pfad/zu/quelle.tar}} --wildcards "{{*.html}}"
```
{% endraw %}