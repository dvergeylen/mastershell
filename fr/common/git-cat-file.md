---
layout: default
title: "git cat-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cat-file">
  <a href="/fr/common/git-cat-file.html">git cat-file</a> <a href="#git-cat-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fournir des informations sur le contenu ou le type et la taille des objets du dépôt Git.
> Plus d'informations : <https://git-scm.com/docs/git-cat-file>.

#### Obtenir la taille [s] du commit HEAD en octets :
```shell
git cat-file -s HEAD
```
#### Obtenir le type [t] (blob, tree, commit, tag) d'un objet Git spécifié :
```shell
git cat-file -t {{8c442dc3}}
```
#### Affiche le contenu [p] d'un objet Git basé sur son type :
```shell
git cat-file -p {{HEAD~2}}
```
{% endraw %}