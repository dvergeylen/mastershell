---
layout: default
title: "git bisect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bisect">
  <a href="/de/common/git-bisect.html">git bisect</a> <a href="#git-bisect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Benuzt binäre Suche um den commit ausfindig zu machen, welcher einen Fehler beinhaltet.
> Git springt im Commit-Graph automatisch vor und zurück, um den fehlerhaften Commit schrittweise einzugrenzen zu können.
> Weitere Informationen: <https://git-scm.com/docs/git-bisect>.

#### Starte eine Bisect-Session in einem Commit-Bereich, der durch einen bekannten fehlerhaften Commit und einen sauberen Commit begrenzt wird:
```shell
git bisect start {{fehlerhafter_commit}} {{sauberer_commit}}
```
#### Prüfe jeden Commit, den `git bisect` auswählt, und kennzeichne ihn mit "gut" oder "schlecht":
```shell
git bisect {{good|bad}}
```
#### Wechsle zum vorherigen Branch zurück, nachdem der fehlerhafte Commit lokalisiert wurde:
```shell
git bisect reset
```
#### Überspringe einen Commit während der Bisect-Session (z.B. einen, der die Tests aufgrund eines anderen Problems nicht bestanden hat):
```shell
git bisect skip
```
{% endraw %}