---
layout: default
title: "git pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pull">
  <a href="/fr/common/git-pull.html">git pull</a> <a href="#git-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Récupère une branche depuis le serveur distant et la fusionne dans la branche local.
> Plus d'informations : <https://git-scm.com/docs/git-pull>.

#### Télécharge les changements depuis le serveur distant par défaut et fusionne les :
```shell
git pull
```
#### Télécharge les changements depuis le serveur distant par défaut et applique les changements locaux par dessus :
```shell
git pull --rebase
```
#### Télécharge les changements depuis un serveur et une branche distante, puis fusionne les dans HEAD :
```shell
git pull {{nom_distant}} {{branche}}
```
{% endraw %}