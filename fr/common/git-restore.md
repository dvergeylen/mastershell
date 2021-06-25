---
layout: default
title: "git restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-restore">
  <a href="/fr/common/git-restore.html">git restore</a> <a href="#git-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restaurez les fichiers de l'arborescence de travail. Nécessite la version 2.23+ de Git.
> Voir aussi `git checkout`.
> Plus d'informations : <https://git-scm.com/docs/git-restore>.

#### Restaurer un fichier supprimé à partir du contenu du commit actuel (HEAD) :
```shell
git restore {{chemin/vers/fichier}}
```
#### Restaurer un fichier a la version d'un commit spécifié :
```shell
git restore --source {{commit}} {{chemin/vers/fichier}}
```
#### Annulez toutes les modifications non validées des fichiers suivis, en revenant au HEAD :
```shell
git restore .
```
{% endraw %}