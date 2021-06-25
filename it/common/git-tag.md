---
layout: default
title: "git tag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-tag">
  <a href="/it/common/git-tag.html">git tag</a> <a href="#git-tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea, elenca, cancella o verifica tag.
> Un tag è un riferimento statico a uno specifico commit.
> Maggiori informazioni: <https://git-scm.com/docs/git-tag>.

#### Mostra tutti i tag:
```shell
git tag
```
#### Crea un tag con un nome, puntandolo al commit corrente:
```shell
git tag {{nome_tag}}
```
#### Crea un tag con un nome, puntandolo ad un dato commit:
```shell
git tag {{nome_tag}} {{commit}}
```
#### Crea un tag annotandolo con un messaggio:
```shell
git tag {{nome_tag}} -m {{messaggio_tag}}
```
#### Cancella un tag, dato il suo nome:
```shell
git tag -d {{nome_tag}}
```
#### Scarica tag aggiornati da upstream:
```shell
git fetch --tags
```
#### Mostra tutti i tag i cui predecessori includono uno specifico commit:
```shell
git tag --contains {{commit}}
```
{% endraw %}