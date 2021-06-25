---
layout: default
title: "apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt">
  <a href="/de/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian und Ubuntu Paket Management Tool.
> Empfohlene Alternative zu apt-get seit Ubuntu 16.04.
> Weitere Informationen: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Aktualisiere die Liste der Paketquellen (es wird empfohlen, diesen Befehl zu Beginn auszuführen):
```shell
sudo apt update
```
#### Suche nach einem Paket:
```shell
apt search {{paket}}
```
#### Zeige Informationen über ein Paket:
```shell
apt show {{paket}}
```
#### Installiere ein Paket oder aktualisiere es zur neusten Version:
```shell
sudo apt install {{paket}}
```
#### Entferne ein Paket:
```shell
sudo apt remove {{paket}}
```
#### Aktualisiere alle installierten Pakete auf die neueste Version:
```shell
sudo apt upgrade
```
#### Liste alle Pakete auf:
```shell
apt list
```
#### Liste alle installierten Pakete auf:
```shell
apt list --installed
```
{% endraw %}