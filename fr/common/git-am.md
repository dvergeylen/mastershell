---
layout: default
title: "git am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-am">
  <a href="/fr/common/git-am.html">git am</a> <a href="#git-am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Appliquer des fichiers de "patch" Git. Utile lorsque l'on reçoit des commits par email.
> Voir aussi `git format-patch`, pour générer des fichiers de patch.
> Plus d'informations : <https://git-scm.com/docs/git-am>.

#### Appliquer un fichier de patch :
```shell
git am {{chemin/vers/fichier.patch}}
```
#### Annuler l'application d'un fichier de patch :
```shell
git am --abort
```
#### Appliquer autant de fichiers de correctif que possible, en enregistrant les morceaux échoués pour rejeter le fichier :
```shell
git am --reject {{chemin/vers/fichier.patch}}
```
{% endraw %}