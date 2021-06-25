---
layout: default
title: "git ls-tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-tree">
  <a href="/fr/common/git-ls-tree.html">git ls-tree</a> <a href="#git-ls-tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lister le contenu d'un arbre.
> Plus d'informations : <https://git-scm.com/docs/git-ls-tree>.

#### Lister le contenu de l'arbre dans la branche :
```shell
git ls-tree {{nom_de_branche}}
```
#### Lister le contenu de l'arbre dans le commit, récursif avec les sous-arbres :
```shell
git ls-tree -r {{commit_hash}}
```
#### Lister uniquement les noms de fichiers de l'arbre dans un commit :
```shell
git ls-tree --name-only {{commit_hash}}
```
{% endraw %}