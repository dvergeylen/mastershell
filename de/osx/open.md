---
layout: default
title: "open"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="open">
  <a href="/de/osx/open.html">open</a> <a href="#open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Öffne Dateien, Verzeichnisse und Anwendungen.

#### Öffne eine Datei in der zugehörigen Anwendung:
```shell
open {{pfad/zu/datei}}
```
#### Führe eine grafische macOS-Anwendung aus:
```shell
open -a {{anwendung}}
```
#### Führe eine grafische macOS-Anwendung basierend auf der Bundle-Kennung aus (siehe `osascript` für eine einfache Möglichkeit, diese zu identifizieren):
```shell
open -b {{com.domain.anwendung}}
```
#### Öffne das aktuelle Verzeichnis im Finder:
```shell
open .
```
#### Zeige eine Datei im Finder an:
```shell
open -R {{pfad/zu/datei}}
```
#### Öffne alle Dateien einer bestimmten Erweiterung im aktuellen Verzeichnis mit der zugehörigen Anwendung:
```shell
open {{*.ext}}
```
{% endraw %}