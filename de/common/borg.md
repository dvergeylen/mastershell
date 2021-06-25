---
layout: default
title: "borg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="borg">
  <a href="/de/common/borg.html">borg</a> <a href="#borg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deduplizierendes Sicherungswerkzeug.
> Erstellt lokale oder entfernte Sicherungen, die als Dateisysteme einhängbar sind.
> Weitere Informationen: <https://borgbackup.readthedocs.io/en/stable/usage/general.html>.

#### Initialisiere ein lokales Repository:
```shell
borg init {{pfad/zu/repo_verzeichnis}}
```
#### Sichere ein Verzeichnis in das Repository und erstelle ein Archiv mit dem Namen "Montag":
```shell
borg create --progress {{pfad/zu/repo_verzeichnis}}::{{Montag}} {{pfad/zu/quell_verzeichnis}}
```
#### Liste alle Archive in einem Repository auf:
```shell
borg list {{pfad/zu/repo_verzeichnis}}
```
#### Extrahiere ein bestimmtes Verzeichnis aus dem "Montag"-Archiv in einem entfernten Repository, unter Ausschluss aller `*.ext`-Dateien:
```shell
borg extract {{benutzer}}@{{host}}:{{pfad/zu/repo_verzeichnis}}::{{Montag}} {{pfad/zu/ziel_verzeichnis} --exclude '{{*.ext}}'
```
#### Bereinige ein Repository, indem alle Archive gelöscht werden, die älter als 7 Tage sind und Änderungen aufweisen:
```shell
borg prune --keep-within {{7d}} --list {{pfad/zu/repo_verzeichnis}}
```
#### Hänge ein Repository als FUSE-Dateisystem ein:
```shell
borg mount {{pfad/zu/repo_verzeichnis}}::{{Montag}} {{pfad/zu/mountpoint}}
```
#### Zeige Hilfe zur Erstellung von Archiven an:
```shell
borg create --help
```
{% endraw %}