---
layout: default
title: "git rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rm">
  <a href="/de/common/git-rm.html">git rm</a> <a href="#git-rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Entferne Dateien aus dem Index des Repositories und vom lokalen Dateisystem.
> Weitere Informationen: <https://git-scm.com/docs/git-rm>.

#### Entferne eine Datei aus dem Index und vom lokalen Dateisystem:
```shell
git rm {{pfad/zu/datei}}
```
#### Entferne ein Verzeichnis:
```shell
git rm -r {{pfad/zu/verzeichnis}}
```
#### Entferne eine Datei aus dem Index des Repositories, aber behalte sie lokal:
```shell
git rm --cached {{pfad/zu/datei}}
```
{% endraw %}