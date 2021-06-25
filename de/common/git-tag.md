---
layout: default
title: "git tag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-tag">
  <a href="/de/common/git-tag.html">git tag</a> <a href="#git-tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle, lösche, überprüfe und liste Tags auf.
> Weitere Informationen: <https://git-scm.com/docs/git-tag>.

#### Liste alle Tags auf:
```shell
git tag
```
#### Erstelle einen Tag mit Namen, welcher auf den aktuellen Commit zeigt:
```shell
git tag {{tag_name}}
```
#### Erstelle einen Tag mit Namen, welcher auf einen bestimmten Commit zeigt:
```shell
git tag {{tag_name}} {{commit}}
```
#### Erstelle einen Tag mit Anmerkung:
```shell
git tag {{tag_name}} -m {{anmkerung}}
```
#### Lösche einen Tag mit bestimmten Namen:
```shell
git tag -d {{tag_name}}
```
#### Lade die aktualisierten Tags aus dem Upstream:
```shell
git fetch --tags
```
#### Liste alle Tags auf, bei denen sich in den vorangegangenen Commits ein bestimmter Commit findet:
```shell
git tag --contains {{commit}}
```
{% endraw %}