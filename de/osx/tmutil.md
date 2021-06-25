---
layout: default
title: "tmutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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