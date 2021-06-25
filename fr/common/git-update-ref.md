---
layout: default
title: "git update-ref"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-update-ref">
  <a href="/fr/common/git-update-ref.html">git update-ref</a> <a href="#git-update-ref"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commande Git pour créer, mettre à jour et supprimer des références Git.
> Plus d'informations : <https://git-scm.com/docs/git-update-ref>.

#### Supprimer une référence, utile pour la réinitialisation du premier commit :
```shell
git update-ref -d {{HEAD}}
```
#### Mettre a jour une référence avec un message :
```shell
git update-ref -m {{message}} {{HEAD}} {{4e95e05}}
```
{% endraw %}