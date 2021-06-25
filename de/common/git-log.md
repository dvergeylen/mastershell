---
layout: default
title: "git log"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-log">
  <a href="/de/common/git-log.html">git log</a> <a href="#git-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeigt die Commit-Historie an.
> Weitere Informationen: <https://git-scm.com/docs/git-log>.

#### Zeige die Sequenz der Commits des Git-Repository im aktuellen Verzeichnis, beginnend mit dem aktuellen, an.
```shell
git log
```
#### Zeige die Historie einer bestimmten Datei oder eines Verzeichnisses, inklusive Unterschiede, an:
```shell
git log -p {{pfad/zu/datei_oder_verzeichnis}}
```
#### Zeige einen Überblick der Commits an und welche Dateien jeweils verändert wurden:
```shell
git log --stat
```
#### Zeige einen Graphen von Commits im aktuellen Branch, wobei jeweils nur die erste Zeile der Commit-Nachricht angezeigt wird:
```shell
git log --oneline --graph
```
#### Zeige einen Graphen von allen Commits, Tags und Branches im gesamten Repository:
```shell
git log --oneline --decorate --all --graph
```
#### Zeige nur Commits, deren Commit-Nachricht einen bestimmten Text enthalten (Ohne Beachtung von Groß- und Kleinschreibung):
```shell
git log -i --grep {{text}}
```
#### Zeige die letzten N Commits eines bestimmten Autors:
```shell
git log -n {{anzahl}} --author={{autor}}
```
#### Zeige alle Commits zwischen zwei Zeitpunkten an:
```shell
git log --before={{datum}} --after={{datum}}
```
{% endraw %}