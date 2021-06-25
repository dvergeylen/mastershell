---
layout: default
title: "git branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-branch">
  <a href="/it/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Il principale comando Git per lavorare con i rami.
> Maggiori informazioni: <https://git-scm.com/docs/git-branch>.

#### Elenca i rami locali. Il ramo corrente è evidenziato da un `*`:
```shell
git branch
```
#### Elenca tutti i rami (locali e remoti):
```shell
git branch -a
```
#### Crea un nuovo ramo a partire dal commit corrente:
```shell
git branch {{nome_ramo}}
```
#### Crea un nuovo ramo a partire dal commit specificato:
```shell
git branch {{nome_ramo}} {{hash_commit}}
```
#### Rinomina un ramo (non applicabile sul ramo corrente):
```shell
git branch -m {{vecchio_nome}} {{nuovo_nome}}
```
#### Cancella un ramo locale (non applicabile sul ramo corrente):
```shell
git branch -d {{nome_ramo}}
```
{% endraw %}