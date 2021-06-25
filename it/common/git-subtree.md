---
layout: default
title: "git subtree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-subtree">
  <a href="/it/common/git-subtree.html">git subtree</a> <a href="#git-subtree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per gestire le dipendenze di un progetto come progetti secondari.
> Maggiori informazioni: <https://manpages.debian.org/testing/git-man/git-subtree.1.en.html>.

#### Aggiungi un repository Git come albero secondario:
```shell
git subtree add --prefix={{percorso/alla/cartella/}} --squash {{url_repository}} {{master}}
```
#### Aggiorna l'albero secondario di un repository al suo commit più recente:
```shell
git subtree pull --prefix={{percorso/alla/cartella/}} {{url_repository}} {{master}}
```
#### Unisci un albero secondario al ramo principale (master):
```shell
git subtree merge --prefix={{percorso/alla/cartella/}} --squash {{url_repository}} {{master}}
```
#### Invia commit all'albero secondario di un repository:
```shell
git subtree push --prefix={{percorso/alla/cartella/}} {{url_repository}} {{master}}
```
#### Estrai la cronologia di un nuovo progetto dalla cronologia di un albero secondario:
```shell
git subtree split --prefix={{percorso/alla/cartella/}} {{url_repository}} -b {{nome_ramo}}
```
{% endraw %}