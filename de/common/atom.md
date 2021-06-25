---
layout: default
title: "atom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atom">
  <a href="/de/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein plattformübergreifender erweiterbarer Texteditor.
> Erweiterungen werden durch `apm` verwaltet.
> Weitere Informationen: <https://atom.io/>.

#### Öffne eine Datei oder ein Verzeichnis:
```shell
atom {{pfad/zu/datei_oder_verzeichnis}}
```
#### Öffne eine Datei oder ein Verzeichnis in einem neuen Fenster:
```shell
atom -n {{pfad/zu/datei_oder_verzeichnis}}
```
#### Öffne eine Datei oder ein Verzeichnis in einem vorhandenen Fenster:
```shell
atom --add {{pfad/zu/datei_oder_verzeichnis}}
```
#### Starte Atom im sicheren Modus (Es werden keine zusätzlichen Pakete geladen):
```shell
atom --safe
```
#### Verhindert, dass sich Atom in den Hintergrund absetzt und hält es mit dem Terminal verbunden:
```shell
atom --foreground
```
#### Wartet, bis Atom geschlossen wurde, bevor die Eingabeaufforderung wieder aktiv wird (Nützlich als `git commit` Editor):
```shell
atom --wait
```
{% endraw %}