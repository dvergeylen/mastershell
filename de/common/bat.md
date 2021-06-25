---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/de/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ausgabe und Verkettung von einzelnen Dateien.
> Ein `cat`-Ersatz mit Syntax-Hervorhebung und Git-Integration.

#### Gib den Inhalt einer Datei in stdout aus:
```shell
bat {{pfad/zu/datei}}
```
#### Verkette mehrere Dateien zu eine Zieldatei:
```shell
bat {{pfad/zu/datei1}} {{pfad/zu/datei2}} > {{pfad/zu/ziel_datei}}
```
#### Hänge mehrere Dateien an eine Zieldatei an:
```shell
bat {{pfad/zu/datei1}} {{pfad/zu/datei2}} >> {{pfad/zu/ziel_datei}}
```
#### Nummeriere alle ausgegebenen Zeilen:
```shell
bat -n {{pfad/zu/datei}}
```
#### Hebe den Syntax einer JSON-Datei hervor:
```shell
bat --language {{json}} {{pfad/zu/datei.json}}
```
#### Zeige alle unterstüzten Sprachen an:
```shell
bat --list-languages
```
{% endraw %}