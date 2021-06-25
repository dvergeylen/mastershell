---
layout: default
title: "tlmgr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tlmgr">
  <a href="/de/common/tlmgr.html">tlmgr</a> <a href="#tlmgr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Packages und Konfigurationen einer existierenden TeX Live Installation.
> Weitere Informationen: <https://www.tug.org/texlive/tlmgr.html>.

#### Installiere ein Package und seine Abhängigkeiten:
```shell
tlmgr install {{package}}
```
#### Entferne ein Package und seine Abhängigkeiten:
```shell
tlmgr remove {{package}}
```
#### Zeige Informationen über ein Pagkage an:
```shell
tlmgr info {{package}}
```
#### Aktualisiere alle Packages:
```shell
tlmgr update --all
```
#### Zeige mögliche Aktualisierungen an, ohne Änderungen vorzunehmen:
```shell
tlmgr update --list
```
#### Starte die graphische Oberfläche von tlmgr:
```shell
tlmgr gui
```
#### Liste alle Tex Live Konfigurationen auf:
```shell
tlmgr conf
```
{% endraw %}