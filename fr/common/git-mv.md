---
layout: default
title: "git mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mv">
  <a href="/fr/common/git-mv.html">git mv</a> <a href="#git-mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Déplacer ou renommer des fichiers inscrits dans l'index.
> Plus d'informations : <https://git-scm.com/docs/git-mv>.

#### Déplace les fichiers dans l'index Git, valide au prochain commit :
```shell
git mv {{chemin/vers/fichier}} {{new/path/to/file}}
```
#### Renome un fichier et met a jour l'index, valide au prochain commit :
```shell
git mv {{filename}} {{new_filename}}
```
#### Force l'écrasement d'un fichier :
```shell
git mv --force {{file}} {{cible}}
```
{% endraw %}