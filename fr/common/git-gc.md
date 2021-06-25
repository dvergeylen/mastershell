---
layout: default
title: "git gc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-gc">
  <a href="/fr/common/git-gc.html">git gc</a> <a href="#git-gc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimise le dépôt local git en nettoyant les fichiers inutiles.
> Plus d'informations : <https://git-scm.com/docs/git-gc>.

#### Optimise le dépôt :
```shell
git gc
```
#### Optimise le dépôt plus agressivement, plus long :
```shell
git gc --aggressive
```
#### Afficher les objets à supprimer :
```shell
git gc --no-prune
```
#### Supprime tout les objets trouvés sans les afficher sur la sortie standard :
```shell
git gc --quiet
```
#### Afficher le manuel :
```shell
git gc --help
```
{% endraw %}