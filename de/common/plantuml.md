---
layout: default
title: "plantuml"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="plantuml">
  <a href="/de/common/plantuml.html">plantuml</a> <a href="#plantuml"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle UML-Diagramme aus einer reinen Textsprache und rendere sie in verschiedenen Formaten.
> Weitere Informationen: <https://plantuml.com/en/command-line>.

#### Rendere Diagramme im Standardformat (PNG):
```shell
plantuml {{pfad/zu/diagramm1.puml}} {{pfad/zu/diagramm2.puml}}
```
#### Rendere eine Diagramm im vorgegebenen Format (z.B. `png`, `pdf`, `svg`, `txt`):
```shell
plantuml -t {{format}} {{pfad/zu/diagramm.puml}}
```
#### Rendere alle Diagramme eines Verzeichnisses:
```shell
plantuml {{pfad/zu/verzeichnis}}
```
#### Rendere ein Diagramm in ein bistimmtes Ausgabeverzeichnis:
```shell
plantuml -o {{pfad/zu/verzeichnis}} {{pfad/zu/diagramm.puml}}
```
#### Rendere ein Diagramm mit einer bestimmten Konfigurationsdatei:
```shell
plantuml -config {{pfad/zu/konfig.cfg}} {{pfad/zu/diagramm.puml}}
```
#### Zeige Hilfe an:
```shell
plantuml -help
```
{% endraw %}