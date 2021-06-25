---
layout: default
title: "apt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-get">
  <a href="/de/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian und Ubuntu Paket Management Tool.
> Suche mit `apt-cache` nach Paketen.
> Weitere Informationen: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Aktualisiere die Liste der Paketquellen (es wird empfohlen diesen Befehl zu Begin auszuführen):
```shell
apt-get update
```
#### Installiere ein Paket oder aktualisiere es zur neuesten Version:
```shell
apt-get install {{paket}}
```
#### Entferne ein Paket:
```shell
apt-get remove {{paket}}
```
#### Entferne ein Paket und die dazugehörigen Konfigurationen:
```shell
apt-get purge {{paket}}
```
#### Aktualisiere alle Pakete auf die neueste Version:
```shell
apt-get upgrade
```
#### Reinige das Repository
```shell
apt-get autoclean
```
#### Entferne alle Pakete, die nicht mehr benötigt werden:
```shell
apt-get autoremove
```
#### Aktualisiere alle Pakete (wie `upgrade`), aber entfernt alle obsoleten Pakete:
```shell
apt-get dist-upgrade
```
{% endraw %}