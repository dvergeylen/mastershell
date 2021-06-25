---
layout: default
title: "git add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-add">
  <a href="/it/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aggiungi file nuovi o modificati all'area di stage.
> Maggiori informazioni: <https://git-scm.com/docs/git-add>.

#### Aggiungi un file all'area di stage:
```shell
git add {{percorso/al/file}}
```
#### Aggiungi tutti i file (tracciati e non tracciati):
```shell
git add -A
```
#### Aggiungi solo i file già tracciati:
```shell
git add -u
```
#### Aggiungi anche i file ignorati:
```shell
git add -f
```
#### Aggiungi parti di un file in modo interattivo:
```shell
git add -p {{percorso/al/file}}
```
{% endraw %}