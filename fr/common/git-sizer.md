---
layout: default
title: "git sizer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-sizer">
  <a href="/fr/common/git-sizer.html">git sizer</a> <a href="#git-sizer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calcule diverses métriques de taille de dépôt Git et vous alerte de tout ce qui pourrait causer des problèmes ou des inconvénients.
> Plus d'informations : <https://github.com/github/git-sizer>.

#### Signaler uniquement les statistiques dont le niveau de préoccupation est supérieur à 0 :
```shell
git sizer
```
#### Signaler toutes les statistiques :
```shell
git sizer -v
```
#### Afficher les options additionnelles :
```shell
git sizer -h
```
{% endraw %}