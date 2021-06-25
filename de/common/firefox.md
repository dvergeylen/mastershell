---
layout: default
title: "firefox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="firefox">
  <a href="/de/common/firefox.html">firefox</a> <a href="#firefox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein gratis Open Source Internet Browser.
> Weitere Informationen: <https://developer.mozilla.org/en-US/docs/Mozilla/Command_Line_Options>.

#### Starte Firefox und öffne eine Website:
```shell
firefox {{https://www.duckduckgo.com}}
```
#### Öffne ein neues Fenster:
```shell
firefox --new-window {{https://www.duckduckgo.com}}
```
#### Öffne ein privates (Icognito) Fenster:
```shell
firefox --private-window
```
#### Suche nach "wikipedia" mit der Standard-Suchmaschine:
```shell
firefox --search "{{wikipedia}}"
```
#### Starte Firefox im sicheren Modus (alle Erweiterungen sind deaktiviert):
```shell
firefox --safe-mode
```
#### Erstelle eine Bildschirmaufnahme einer Website, ohne die GUI zu starten:
```shell
firefox --headless --screenshot {{pfad/zu/ausgabedatei.png}} {{https://beispiel.de/}}
```
#### Verwende ein bestimmtes Profil um mehrere einzelne Instanzen gleichzeitig laufen zu lassen:
```shell
firefox --profile {{pfad/zu/verzeichnis}} {{https://beispiel.de/}}
```
#### Lege Firefox als Standard-Browser fest:
```shell
firefox --setDefaultBrowser
```
{% endraw %}