---
layout: default
title: "git reset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reset">
  <a href="/it/common/git-reset.html">git reset</a> <a href="#git-reset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Annulla commit o rimuovi modifiche dall'area di stage, reimpostando l'HEAD corrente su uno specifico stato.
> Se viene fornito un percorso, il comando reset si interpreta come "rimuovi dall'area di stage"; se viene fornito l'hash di un commit o un ramo, si interpreta come "annulla commit".
> Maggiori informazioni: <https://git-scm.com/docs/git-reset>.

#### Rimuovi tutto dall'area di stage:
```shell
git reset
```
#### Rimuovi dall'area di stage uno o più file:
```shell
git reset {{percorso/al/file1}} {{percorso/al/file2}}
```
#### Rimuovi dall'area di stage solo alcune porzioni di un file in modo interattivo:
```shell
git reset --patch {{percorso/al/file}}
```
#### Annulla l'ultimo commit, preservando tutte le modifiche nel filesystem:
```shell
git reset HEAD~
```
#### Annulla gli ultimi due commit, aggiungendo all'area di stage le modifiche relative:
```shell
git reset --soft HEAD~2
```
#### Annulla le modifiche non committate, indipendentemente se siano presenti nell'area di stage o meno (usa `git checkout` per queste ultime):
```shell
git reset --hard
```
#### Reimposta il repository su un dato commit, annullando qualsiasi tipo di modifica precedente:
```shell
git reset --hard {{commit}}
```
{% endraw %}