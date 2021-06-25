---
layout: default
title: "git show"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show">
  <a href="/it/common/git-show.html">git show</a> <a href="#git-show"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra vari tipi di oggetti Git (commit, tag, etc.).
> Maggiori informazioni: <https://git-scm.com/docs/git-show>.

#### Mostra informazioni sull'ultimo commit (hash, messaggio, modifiche, ed altri metadati):
```shell
git show
```
#### Mostra informazioni su un dato commit:
```shell
git show {{commit}}
```
#### Mostra informazioni sul commit associato ad un tag specifico:
```shell
git show {{tag}}
```
#### Mostra informazioni sul terzo commit dalla cima del ramo:
```shell
git show {{ramo}}~{{3}}
```
#### Mostra il messaggio di commit su linea singola, senza mostrare il diff:
```shell
git show --oneline -s {{commit}}
```
#### Mostra solo la lista dei file modificati in un commit:
```shell
git show --stat {{commit}}
```
#### Mostra il contenuto di un file ad una data revisione (ad esempio, in un ramo, tag o commit):
```shell
git show {{revisione}}:{{percorso/al/file}}
```
{% endraw %}