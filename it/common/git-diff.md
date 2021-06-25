---
layout: default
title: "git diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-diff">
  <a href="/it/common/git-diff.html">git diff</a> <a href="#git-diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra le modifiche ai file tracciati.
> Maggiori informazioni: <https://git-scm.com/docs/git-diff>.

#### Mostra le modifiche non ancora nell'area di stage:
```shell
git diff
```
#### Mostra tutte le modifiche non ancora salvate in un commit (incluse quelle nell'area di stage):
```shell
git diff HEAD
```
#### Mostra solo le modifiche nell'area di stage (aggiunte, ma non ancora committate):
```shell
git diff --staged
```
#### Mostra le modifiche di tutti i commit a partire da una certa data/ora (un'espressione temporale come "1 week 2 days" o una data ISO):
```shell
git diff 'HEAD@{3 months|weeks|days|hours|seconds ago}'
```
#### Mostra solo i nomi dei file modificati a partire da un dato commit:
```shell
git diff --name-only {{commit}}
```
#### Stampa un riepilogo dei file creati, rinominati o la cui modalità è cambiata a partire da un dato commit:
```shell
git diff --summary {{commit}}
```
#### Confronta le versioni di un dato file tra due rami o commit:
```shell
git diff {{ramo_1}}..{{ramo_2}} [--] {{percorso/al/file}}
```
#### Confronta le versioni di più file tra il ramo corrente e un altro ramo:
```shell
git diff {{ramo}}:{{percorso/al/file2}} {{percorso/al/file}}
```
{% endraw %}