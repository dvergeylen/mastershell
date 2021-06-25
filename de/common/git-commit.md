---
layout: default
title: "git commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit">
  <a href="/de/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Committe Dateien in ein Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-commit>.

#### Committe gestagten Dateien zum Repository mit einer Nachricht:
```shell
git commit -m "{{nachricht}}"
```
#### Committe alle gestagten Dateien zum Repository mit einer Nachricht aus einer Datei:
```shell
git commit --file {{pfad/zu/commit_nachricht_datei}}
```
#### Stage alle modifizierten Dateien und committe sie mit einer Nachricht:
```shell
git commit -a -m "{{nachricht}}"
```
#### Ersetze den letzten Commit mit den gerade auf dem Stage liegenden Änderungen:
```shell
git commit --amend
```
#### Comitte nur spezifische Dateien (die Dateien müssen schon auf dem Stage liegen):
```shell
git commit {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
{% endraw %}