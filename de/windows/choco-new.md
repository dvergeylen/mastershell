---
layout: default
title: "choco new"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-new">
  <a href="/de/windows/choco-new.html">choco new</a> <a href="#choco-new"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle neue Paket-Beschreibungs-Dateien mit Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-new>.

#### Erstelle ein neues Grundgerüst für ein Paket:
```shell
choco new {{paket_name}}
```
#### Erstelle ein neues Paket mit einer bestimmten Version:
```shell
choco new {{paket_name}} --version {{version}}
```
#### Erstelle ein neues Paket mit einem bestimmten Betreuer*innen-Namen:
```shell
choco new {{paket_name}} --maintainer {{betreuer*innen_name}}
```
#### Erstelle ein neues Paket in einem bestimmten Ausgabe-Verzeichnis:
```shell
choco new {{paket_name}} --output-directory {{pfad/zu/verzeichnis}}
```
#### Erstelle ein neues Paket mit verschiedenen URLs für die 32-Bit und 64-Bit Installationsroutinen:
```shell
choco new {{paket_name}} url="{{url}}" url64="{{url}}"
```
{% endraw %}