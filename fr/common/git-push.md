---
layout: default
title: "git push"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-push">
  <a href="/fr/common/git-push.html">git push</a> <a href="#git-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pousse les commits vers un dépôt distant.
> Plus d'informations : <https://git-scm.com/docs/git-push>.

#### Envoie les changements locaux dans la branche courante vers sa contrepartie distante :
```shell
git push
```
#### Envoie les changements locaux d'une branche spécifique vers sa contrepartie distante :
```shell
git push {{nom_distant}} {{local_branch}}
```
#### Publie la branche courante vers un dépôt distant, crée le nom de la branche distante :
```shell
git push {{nom_distant}} -u {{branche_distante}}
```
#### Envoi les changements locaux sur toutes les branches locales vers leur contrepartie sur le dépôt distant :
```shell
git push --all {{nom_distant}}
```
#### Supprime une branche dans un dépôt distant :
```shell
git push {{nom_distant}} --delete {{branche_distante}}
```
#### Supprime les branches distantes qui n'ont pas de contrepartie locale :
```shell
git push --prune {{nom_distant}}
```
#### Publie les tags qui ne sont pas sur le dépôt distant :
```shell
git push --tags
```
{% endraw %}