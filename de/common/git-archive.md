---
layout: default
title: "git archive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-archive">
  <a href="/de/common/git-archive.html">git archive</a> <a href="#git-archive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle ein Archiv von Dateien.
> Weitere Informationen: <https://git-scm.com/docs/git-archive>.

#### Erstelle ein tar-Archiv aus dem Inhalt des aktuellen HEAD und gib dieses aus:
```shell
git archive --verbose HEAD
```
#### Erstelle ein zip-Archiv aus dem Inhalt des aktuellen HEAD und gib dieses aus:
```shell
git archive --verbose --format=zip HEAD
```
#### Erstelle ein zip-Archiv aus dem Inhalt des aktuellen HEAD und speichere dieses in eine Datei:
```shell
git archive --verbose --output={{pfad/zu/datei.zip}} HEAD
```
#### Erstelle ein tar-Archiv aus dem Inhalt des letzten Commits eines bestimmten Branches:
```shell
git archive --output={{pfad/zu/datei.tar}} {{branch_name}}
```
#### Erstelle ein tar-Archiv aus dem Inhalt eines bestimmten Verzeichnisses:
```shell
git archive --output={{pfad/zu/datei.tar}} HEAD:{{pfad/zu/verzeichnis}}
```
#### Stelle jeder Datei einen Pfad voran, um sie in einem bestimmten Verzeichnis zu archivieren:
```shell
git archive --output={{pfad/zu/datei.tar}} --prefix={{pfad/zu/verzeichnis}}/ HEAD
```
{% endraw %}