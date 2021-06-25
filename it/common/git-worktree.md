---
layout: default
title: "git worktree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-worktree">
  <a href="/it/common/git-worktree.html">git worktree</a> <a href="#git-worktree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci gli alberi di lavoro collegati allo stesso repository.
> Maggiori informazioni: <https://git-scm.com/docs/git-worktree>.

#### Crea una nuova cartella a partire da uno specifico ramo:
```shell
git worktree add {{percorso/alla/cartella}} {{ramo}}
```
#### Crea una nuova cartella a partire da un nuovo ramo:
```shell
git worktree add {{percorso/alla/cartella}} -b {{nuovo_ramo}}
```
#### Mostra tutte le cartelle di lavoro collegate al repository corrente:
```shell
git worktree list
```
#### Cancella un albero di lavoro (dopo averne cancellato la cartella):
```shell
git worktree prune
```
{% endraw %}