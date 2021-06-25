---
layout: default
title: "git switch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-switch">
  <a href="/de/common/git-switch.html">git switch</a> <a href="#git-switch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wechsle zwischen Branches. Verfügbar ab Git Version 2.23+.
> Siehe auch `git checkout`.
> Weitere Informationen: <https://git-scm.com/docs/git-switch>.

#### Wechsle zu einem existierenden Branch:
```shell
git switch {{branche_name}}
```
#### Erstelle einen neuen Branch und wechsele zu diesem:
```shell
git switch --create {{branch_name}}
```
#### Erstelle einen neuen Branch basierend auf einem existierenden Commit und wechsele zu diesem:
```shell
git switch --create {{branch_name}} {{commit}}
```
#### Wechsele zum vorherigen Branch:
```shell
git switch -
```
#### Wechsele zu einem Branch und aktualisiere alle Submodule entsprechend:
```shell
git switch --recurse-submodules {{branch_name}}
```
#### Wechsele zu einem Branch und merge automatisch den aktuellen Branch und alle Änderungen, die nicht committed wurden:
```shell
git switch --merge {{branch_name}}
```
{% endraw %}