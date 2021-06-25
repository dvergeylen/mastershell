---
layout: default
title: "osx"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#brew-bundle">brew bundle</a>
* <a href="#caffeinate">caffeinate</a>
* <a href="#open">open</a>
* <a href="#tmutil">tmutil</a>

{% raw %}
<h2 id="brew-bundle">
  <a href="/de/osx/brew-bundle.html">brew bundle</a> <a href="#brew-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bundler für Homebrew, Homebrew Cask und den Mac App Store.
> Weitere Informationen: <https://github.com/Homebrew/homebrew-bundle>.

#### Installiere Pakete aus einer Brewfile im aktuellen Pfad:
```shell
brew bundle
```
#### Installiere Pakete aus einer bestimmten Brewfile:
```shell
brew bundle --file={{pfad/zu/brewfile}}
```
#### Gib eine Liste mit allen installierten Paketen aus:
```shell
brew bundle dump
```
#### Deinstalliere Pakete, die nicht in der Brewfile aufgelisted sind:
```shell
brew bundle cleanup --force
```
#### Prüfe, ob von einem Paket die aktuellste Version installiert ist:
```shell
brew bundle check
```
#### Zeige alle Pakete, die in der Brewfile aufgelistet sind:
```shell
brew bundle list --all
```
{% endraw %}{% raw %}
<h2 id="caffeinate">
  <a href="/de/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hindert den Mac daran in den Schlaf-Modus zu gehen.

#### Halte den Mac für 1 Stunde (3600 Sekunden) wach:
```shell
caffeinate -u -t {{3600}}
```
#### Halte den Mac wach, bis ein bestimmter Befehl abgeschlossen ist:
```shell
caffeinate -s {{befehl}}
```
#### Halte den Mac wach, bis `caffeinate` durch Cmd-C beendet wird:
```shell
caffeinate -i
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="tmutil">
  <a href="/de/osx/tmutil.html">tmutil</a> <a href="#tmutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dienstprogramm zum Verwalten von Time Machine-Backups. Die meisten Befehle erfordern Root-Rechte.
> Weitere Informationen: <https://ss64.com/osx/tmutil.html>.

#### Setze ein HFS+ Laufwerk als Backupziel:
```shell
sudo tmutil setdestination {{pfad/zu/einhänge_punkt}}
```
#### Setze eine APF-Freigabe oder SMB-Freigabe als Backupziel:
```shell
sudo tmutil setdestination {{protocol://benutzer[:passwort]@host/share}}
```
#### Hänge das angegebene Ziel an die Liste der Backupziele an:
```shell
sudo tmutil setdestination -a {{ziel}}
```
#### Aktiviere automatische Backups:
```shell
sudo tmutil enable
```
#### Deaktiviere automatische Backups:
```shell
sudo tmutil disable
```
#### Starte ein Backup im Hintergrund, falls nicht bereits eines läuft:
```shell
sudo tmutil startbackup
```
#### Starte ein Backup im Vordergrund, falls nicht bereits eines läuft:
```shell
sudo tmutil startbackup -b
```
#### Stoppe ein laufendes Backup:
```shell
sudo tmutil stopbackup
```
{% endraw %}