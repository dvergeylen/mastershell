---
layout: default
title: "git apply"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-apply">
  <a href="/de/common/git-apply.html">git apply</a> <a href="#git-apply"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Integriere eine Patch-Datei und/oder füge sie zum Index hinzu.
> Weitere Informationen: <https://git-scm.com/docs/git-apply>.

#### Gib Informationen über gepatchte Dateien aus:
```shell
git apply --verbose {{pfad/zu/datei}}
```
#### Integriere die Patch-Datei und füge sie zum Index hinzu:
```shell
git apply --index {{pfad/zu/datei}}
```
#### Integriere eine externe Patch-Datei:
```shell
curl {{https://beispiel.de/datei.patch}} | git apply
```
#### Gib diffstat des Inputs aus und integriere die Patch-Datei:
```shell
git apply --stat --apply {{pfad/zu/datei}}
```
#### Integriere eine Patch-Datei in umgekehrter Reihenfolge:
```shell
git apply --reverse {{pfad/zu/datei}}
```
#### Speichere das Ergebnis einer Patch-Datei im Index, ohne den Arbeitsbaum zu verändern:
```shell
git apply --cache {{pfad/zu/datei}}
```
{% endraw %}