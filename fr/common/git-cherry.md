---
layout: default
title: "git cherry"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cherry">
  <a href="/fr/common/git-cherry.html">git cherry</a> <a href="#git-cherry"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rechercher des commits qui n'ont pas encore été appliqués en amont.
> Plus d'informations : <https://git-scm.com/docs/git-cherry>.

#### Afficher les commits (et leurs messages) avec des commits équivalents en amont :
```shell
git cherry -v
```
#### Spécifiez une branche amont et une branche de rubrique différentes :
```shell
git cherry {{origin}} {{topic}}
```
#### Limiter les commits à ceux dans la limite donnée :
```shell
git cherry {{origin}} {{topic}} {{base}}
```
{% endraw %}