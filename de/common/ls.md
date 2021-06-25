---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/de/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Liste den Inhalt eines Verzeichnisses auf.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/ls>.

#### Liste den Inhalt in einer Datei pro Zeile auf:
```shell
ls -1
```
#### Liste alle Dateien inklusive versteckter Dateien auf:
```shell
ls -a
```
#### Liste alle Dateien mit einem abschließenden `/` bei Verzeichnis-Namen auf:
```shell
ls -F
```
#### Liste alle Dateien mit Berechtigungen, Besitzer, Größe und Änderungsdatum auf:
```shell
ls -la
```
#### Liste alle Dateien mit Dateigröße in für Menschen lesbaren Einheiten (KiB, MiB, GiB):
```shell
ls -lh
```
#### Liste Dateien nach sortiert nach Dateigröße mit größter beginnend auf:
```shell
ls -lS
```
#### Liste alle Dateien sortiert nach dem Änderungsdatum mit ältester beginnend auf:
```shell
ls -ltr
```
{% endraw %}