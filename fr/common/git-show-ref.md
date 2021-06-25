---
layout: default
title: "git show-ref"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show-ref">
  <a href="/fr/common/git-show-ref.html">git show-ref</a> <a href="#git-show-ref"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commande Git pour lister les références.
> Plus d'informations : <https://git-scm.com/docs/git-show-ref>.

#### Affiche toutes les références dans le dépôt :
```shell
git show-ref
```
#### Affiche seulement les références des têtes de branches :
```shell
git show-ref --heads
```
#### Affiche seulement les références de tags :
```shell
git show-ref --tags
```
#### Vérifier l'existence d'une référence :
```shell
git show-ref --verify {{chemin/vers/reference}}
```
{% endraw %}