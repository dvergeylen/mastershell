---
layout: default
title: "git push"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-push">
  <a href="/de/common/git-push.html">git push</a> <a href="#git-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lade Commits in ein Remote-Repository hoch.
> Weitere Informationen: <https://git-scm.com/docs/git-push>.

#### Sende lokale Änderungen des aktuellen Branches zu seinem entfernten Repository (Remote Branch):
```shell
git push
```
#### Sende lokale Änderungen des angegebenen Branches zu seinem entfernten Repository:
```shell
git push {{remote_name}} {{lokaler_branch}}
```
#### Lade den aktuellen Branches in ein entferntes Repository mit Angabe des Namens des entfernten Branches hoch:
```shell
git push {{remote_name}} -u {{remote_branch}}
```
#### Lade Änderungen aller lokalen Branches zu ihrem entfernten Repository hoch:
```shell
git push --all {{remote_name}}
```
#### Lösche einen Branches in einem entfernten Repository:
```shell
git push {{remote_name}} --delete {{remote_branch}}
```
#### Entferne alle remote Branches, welche kein lokales Gegenstück besitzen:
```shell
git push --prune {{remote_name}}
```
#### Veröffentliche Tags, welche noch nicht im entfernten Repository vorhanden sind:
```shell
git push --tags
```
{% endraw %}