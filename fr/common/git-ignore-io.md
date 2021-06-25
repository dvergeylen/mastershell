---
layout: default
title: "git ignore-io"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ignore-io">
  <a href="/fr/common/git-ignore-io.html">git ignore-io</a> <a href="#git-ignore-io"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Générer le fichier .gitignore depuis des templates prédéfinis.
> Plus d'informations : <https://github.com/tj/git-extras/blob/master/Commands.md#git-ignore-io>.

#### Lister les templates disponibles :
```shell
git ignore-io list
```
#### Générer un template .gitignore :
```shell
git ignore-io {{item_a,item_b,item_n}}
```
{% endraw %}