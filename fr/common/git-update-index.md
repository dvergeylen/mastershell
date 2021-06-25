---
layout: default
title: "git update-index"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-update-index">
  <a href="/fr/common/git-update-index.html">git update-index</a> <a href="#git-update-index"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commande Git pour manipuler l'index.
> Plus d'informations : <https://git-scm.com/docs/git-update-index>.

#### Prétendre qu'un fichier modifié est inchangé (`git status` ne l'affichera pas comme modifié) :
```shell
git update-index --skip-worktree {{chemin/vers/fichier_modifié}}
```
{% endraw %}