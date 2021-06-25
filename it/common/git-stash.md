---
layout: default
title: "git stash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stash">
  <a href="/it/common/git-stash.html">git stash</a> <a href="#git-stash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Salva in un'area temporanea (stash) modifiche Git locali.
> Maggiori informazioni: <https://git-scm.com/docs/git-stash>.

#### Salva in un'area temporanea modifiche locali, tranne i file nuovi e non tracciati:
```shell
git stash [push -m {{messaggio_di_stash_opzionale}}]
```
#### Includi nello stash anche i file nuovi e non tracciati:
```shell
git stash -u
```
#### Seleziona per lo stash parti di file modificati in modo interattivo:
```shell
git stash -p
```
#### Elenca tutti gli stash, mostrandone il nome, ramo relativo e messaggio:
```shell
git stash list
```
#### Applica uno stash (quello predefinito è l'ultimo, chiamato stash@{0}):
```shell
git stash apply {{nome_o_commit_stash_opzionale}}
```
#### Applica uno stash (il predefinito è stash@{0}) e rimuovilo dalla lista degli stash se non ha causato conflitti:
```shell
git stash pop {{nome_stash_opzionale}}
```
#### Rimuovi uno stash (il predefinito è stash@{0}):
```shell
git stash drop {{nome_stash_opzionale}}
```
#### Rimuovi tutti gli stash:
```shell
git stash clear
```
{% endraw %}