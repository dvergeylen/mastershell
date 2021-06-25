---
layout: default
title: "git ls-remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-remote">
  <a href="/fr/common/git-ls-remote.html">git ls-remote</a> <a href="#git-ls-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commande Git pour répertorier les références dans un dépôt distant en fonction du nom ou de l'URL.
> Si aucun nom ou URL n'est donné, alors la branche amont configurée sera utilisée, ou l'origine distante si la première n'est pas configurée.
> Plus d'informations : <https://git-scm.com/docs/git-ls-remote>.

#### Afficher les références du dépôt configuré par défaut :
```shell
git ls-remote
```
#### Afficher uniquement les références HEAD du dépôt configuré par défaut :
```shell
git ls-remote --heads
```
#### Afficher uniquement les tags du dépôt configuré par défaut :
```shell
git ls-remote --tags
```
#### Afficher les références du dépôt précisé :
```shell
git ls-remote {{url-du-dépôt}}
```
#### Afficher les références du dépôt précisé filtrés par un motif :
```shell
git ls-remote {{nom-du-dépôt}} "{{motif}}"
```
{% endraw %}