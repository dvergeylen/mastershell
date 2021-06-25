---
layout: default
title: "git fetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fetch">
  <a href="/fr/common/git-fetch.html">git fetch</a> <a href="#git-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cherche les objets et références depuis un dépôt distant.
> Plus d'informations : <https://git-scm.com/docs/git-fetch>.

#### Cherche les dernières modifications du référentiel amont distant par défaut (si configuré) :
```shell
git fetch
```
#### Cherche les nouvelles branches depuis un registre distant :
```shell
git fetch {{nom_distant}}
```
#### Cherche les nouvelles branches depuis tous les registres distants :
```shell
git fetch --all
```
#### Recherche également les tags depuis le registre courant :
```shell
git fetch --tags
```
#### Supprime les références locales de branches ayant été supprimés du registre distant :
```shell
git fetch --prune
```
{% endraw %}