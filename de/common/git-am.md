---
layout: default
title: "git am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-am">
  <a href="/de/common/git-am.html">git am</a> <a href="#git-am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Patch-Dateien integrieren. Nützlich beim Empfang von Commits per E-Mail.
> Siehe auch `git format-patch` zur Erzeugung von Patch-Dateien.
> Weitere Informationen: <https://git-scm.com/docs/git-am>.

#### Integriere eine Patch-Datei:
```shell
git am {{pfad/zu/datei.patch}}
```
#### Brich das Integrieren einer Patch-Datei ab:
```shell
git am --abort
```
#### Integriere so viele Patch-Dateien wie möglich und speichere fehlgeschlagene Teile:
```shell
git am --reject {{pfad/zu/datei.patch}}
```
{% endraw %}