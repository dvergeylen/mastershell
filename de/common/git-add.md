---
layout: default
title: "git add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-add">
  <a href="/de/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Füge Dateien zum Index/Stage hinzu.
> Weitere Informationen: <https://git-scm.com/docs/git-add>.

#### Füge eine bestimmte Datei zum Index hinzu:
```shell
git add {{pfad/zu/datei}}
```
#### Füge alle Dateien zum Index hinzu (nachverfolgte und nicht nachverfolgte):
```shell
git add -A
```
#### Füge nur nachverfolgte Dateien zum Index hinzu (Updaten des Index):
```shell
git add -u
```
#### Füge auch Dateien, welche ignoriert werden (`.gitignore`) hinzu:
```shell
git add -f
```
#### Füge Teile von Dateien zum Index interaktiv hinzu:
```shell
git add -p
```
#### Füge Teile einer bestimmten Datei interaktiv hinzu:
```shell
git add -p {{pfad/zu/datei}}
```
#### Füge Dateien zum Index interaktiv hinzu:
```shell
git add -i
```
{% endraw %}