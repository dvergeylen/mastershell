---
layout: default
title: "scoop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scoop">
  <a href="/de/windows/scoop.html">scoop</a> <a href="#scoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Kommandozeilenwerkzeug, um Windows-Programme (hier bezeichnet als Pakete) zu installieren.
> Weitere Informationen: <https://scoop.sh>.

#### Installiere ein Paket:
```shell
scoop install {{paket}}
```
#### Entferne ein Paket:
```shell
scoop uninstall {{paket}}
```
#### Aktualisiere alle installierten Pakete:
```shell
scoop update *
```
#### Zeige alle installierten Pakete an:
```shell
scoop list
```
#### Zeige Informationen über ein bestimmtes Paket an:
```shell
scoop info {{paket}}
```
#### Suche nach einem Paket:
```shell
scoop search {{paket}}
```
#### Entferne die alten Versionen aller Pakete und lösche den Download-Zwischenspeicher:
```shell
scoop cleanup -k *
```
{% endraw %}