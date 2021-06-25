---
layout: default
title: "dnf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dnf">
  <a href="/de/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Paketmanagement Tool für RHEL, Fedora, und CentOS (ersetzt yum).
> Weitere Informationen: <https://dnf.readthedocs.io/>.

#### Aktualisiere alle Pakete auf die neueste Version:
```shell
sudo dnf upgrade
```
#### Suche nach Paketen:
```shell
dnf search {{schlüsselwort}}
```
#### Zeige Daten über ein bestimmtes Paket an:
```shell
dnf info {{paket}}
```
#### Installiere ein neues Paket:
```shell
sudo dnf install {{paket}}
```
#### Installiere ein neues Paket und antworte "ja" auf alle Fragen:
```shell
sudo dnf -y install {{paket}}
```
#### Entferne ein Paket:
```shell
sudo dnf remove {{paket}}
```
#### Liste alle Pakete auf:
```shell
dnf list --installed
```
#### Zeige welches Paket eine Datei besitzt:
```shell
dnf provides {{pfad/zu/datei}}
```
{% endraw %}