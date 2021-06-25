---
layout: default
title: "git reflog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reflog">
  <a href="/fr/common/git-reflog.html">git reflog</a> <a href="#git-reflog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche un log des changements locaux comme HEAD, tags et branches.
> Plus d'informations : <https://git-scm.com/docs/git-reflog>.

#### Afficher le reflog de HEAD :
```shell
git reflog
```
#### Affiche le reflog d'une branche spécifique :
```shell
git reflog {{nom_de_branche}}
```
#### Affiche les 5 dernières entrées dans le reflog :
```shell
git reflog -n {{5}}
```
{% endraw %}