---
layout: default
title: "git clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clone">
  <a href="/fr/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clone un dépôt existant.
> Plus d'informations : <https://git-scm.com/docs/git-clone>.

#### Clone un dépôt existant :
```shell
git clone {{location_du_depot_distant}}
```
#### Clone un dépôt existant et ses sous-modules :
```shell
git clone --recursive {{location_du_depot_distant}}
```
#### Clone un dépôt local :
```shell
git clone -l
```
#### Clone silencieusement :
```shell
git clone -q
```
#### Clone un dépôt existant en ne récupérant que les 10 commits les plus récents sur la branche par défaut (plus rapide) :
```shell
git clone --depth {{10}} {{location_du_depot_distant}}
```
{% endraw %}