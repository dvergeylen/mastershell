---
layout: default
title: "git show-branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show-branch">
  <a href="/it/common/git-show-branch.html">git show-branch</a> <a href="#git-show-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra rami e relativi commit.
> Maggiori informazioni: <https://git-scm.com/docs/git-show-branch>.

#### Mostra un sommario degli ultimi commit in un ramo:
```shell
git show-branch {{nome_ramo|riferimento|commit}}
```
#### Confronta commit nella cronologia di più commit o rami:
```shell
git show-branch {{nome_ramo|riferimento|commit}}
```
#### Confronta tutti i rami remoti tracciati:
```shell
git show-branch --remotes
```
#### Confronta i rami locali e remoti:
```shell
git show-branch --all
```
#### Mostra gli ultimi commit di tutti i rami:
```shell
git show-branch --all --list
```
#### Confronta un dato ramo con quello corrente:
```shell
git show-branch --current {{commit|nome_ramo|riferimento}}
```
#### Mostra il nome del commit e non il nome relativo:
```shell
git show-branch --sha1-name --current {{current|nome_ramo|riferimento}}
```
#### Mostra un numero aggiuntivo di commit oltre il predecessore comune:
```shell
git show-branch --more {{5}} {{commit|nome_ramo|riferimento}} {{commit|nome_ramo|riferimento}} {{...}}
```
{% endraw %}