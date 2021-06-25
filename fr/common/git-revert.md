---
layout: default
title: "git revert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-revert">
  <a href="/fr/common/git-revert.html">git revert</a> <a href="#git-revert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Créer un nouveau commit qui efface les changements du précédent.
> Plus d'informations : <https://git-scm.com/docs/git-revert>.

#### Crée un commit qui annule les changements du dernier commit :
```shell
git revert {{@}}
```
#### Crée un commit qui annule les changements des 5 dernier commit :
```shell
git revert HEAD~{{4}}
```
#### Crée un commit qui annule les changements de plusieurs commit :
```shell
git revert {{master~5..master~2}}
```
#### Ne pas créer de nouveau commit, remplacer uniquement dans l'arbre courant :
```shell
git revert -n {{0c01a9..9a1743}}
```
{% endraw %}