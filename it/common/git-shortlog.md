---
layout: default
title: "git shortlog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-shortlog">
  <a href="/it/common/git-shortlog.html">git shortlog</a> <a href="#git-shortlog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Riassume l'output di `git log`.
> Maggiori informazioni: <https://git-scm.com/docs/git-shortlog>.

#### Mostra un riassunto dei commit fatti, raggruppati alfabeticamente per nome dell'autore:
```shell
git shortlog
```
#### Mostra un riassunto dei commit fatti, ordinati per numero di commit:
```shell
git shortlog -n
```
#### Mostra un riassunto dei commit fatti, raggruppati per identità dell'utente che ha eseguito il commit (nome e email):
```shell
git shortlog -c
```
#### Mostra un riassunto degli ultimi 5 commit (richiesti sottoforma di intervallo di revisione):
```shell
git shortlog HEAD~{{5}}..HEAD
```
#### Mostra tutti gli utenti, email e numero di commit nel ramo corrente:
```shell
git shortlog -sne
```
#### Mostra tutti gli utenti, email e numero di commit in tutti i rami:
```shell
git shortlog -sne --all
```
{% endraw %}