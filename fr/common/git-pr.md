---
layout: default
title: "git pr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pr">
  <a href="/fr/common/git-pr.html">git pr</a> <a href="#git-pr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Récupère les pull-requests GitHub localement.

#### Récupère une pull-request spécifique :
```shell
git pr {{pr_number}}
```
#### Récupère une pull-request d'un dépôt spécifique :
```shell
git pr {{pr_number}} {{distant}}
```
#### Récupère une pull-request depuis son URL :
```shell
git pr {{url}}
```
#### Nettoie les branches de pull-requests terminées :
```shell
git pr clean
```
{% endraw %}