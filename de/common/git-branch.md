---
layout: default
title: "git branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-branch">
  <a href="/de/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte und Arbeite mit Git Branches.
> Weitere Informationen: <https://git-scm.com/docs/git-branch>.

#### Liste alle lokalen Branches auf. Der momentan aktive (ausgecheckte) Branch wird mit `*` markiert:
```shell
git branch
```
#### Liste alle Branches auf (Lokal und Remote):
```shell
git branch -a
```
#### Zeige den Namen des aktuellen Branches:
```shell
git branch --show-current
```
#### Erstelle einen neuen Branch auf Basis des letzten Commits:
```shell
git branch {{branch_name}}
```
#### Erstelle einen neuen Branch auf Basis eines bestimmten Commits:
```shell
git branch {{branch_name}} {{commit_hash}}
```
#### Benenne einen Branches um (der Branch muss nicht ausgecheckt sein):
```shell
git branch -m {{alter_branch_name}} {{neuer_branch_name}}
```
#### Lösche einen lokalen Branch (der Branch muss nicht ausgecheckt sein):
```shell
git branch -d {{branch_name}}
```
#### Lösche einen remote-Branch:
```shell
git push {{remote_name}} --delete {{remote_branch_name}}
```
{% endraw %}