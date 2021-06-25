---
layout: default
title: "exa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exa">
  <a href="/de/common/exa.html">exa</a> <a href="#exa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein moderner Ersatz für `ls` (Verzeichnisinhalte auflisten).
> Weitere Informationen: <https://the.exa.website>.

#### Liste eine Datei pro Zeile auf:
```shell
exa --oneline
```
#### Liste alle Dateien auf, einschließlich versteckter Dateien:
```shell
exa --all
```
#### Liste alle Dateien im langen Format auf (Berechtigungen, Eigentümer, Größe und Änderungsdatum):
```shell
exa --long --all
```
#### Liste Dateien nach Größe absteigend sortiert auf:
```shell
exa --reverse --sort={{size}}
```
#### Zeige Dateien in einer Baumstruktur an, die drei Ebenen tief ist:
```shell
exa --long --tree --level={{3}}
```
#### Liste Dateien nach Änderungsdatum aufsteigend sortiert auf:
```shell
exa --long --sort={{modified}}
```
{% endraw %}