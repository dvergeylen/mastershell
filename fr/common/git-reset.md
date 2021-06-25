---
layout: default
title: "git reset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reset">
  <a href="/fr/common/git-reset.html">git reset</a> <a href="#git-reset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enlève des commits ou des changements en réinitialisant la tête Git à l'état spécifié.
> Si un chemin est passé en paramètre, Git reset fonctionne comme «unstage».
> Si un hash de commit est passé en paramètre, Git reset annule les commits jusqu'à ce dernier.
> Plus d'informations : <https://git-scm.com/docs/git-reset>.

#### Tout enlever de la *zone de stage* :
```shell
git reset
```
#### Enlever des fichiers spécifiques de la *zone de stage* :
```shell
git reset {{chemin/vers/fichier(s)}}
```
#### Enlever, en mode interactif, des fichiers spécifiques de l’index :
```shell
git reset --patch {{chemin/vers/fichier}}
```
#### Annuler le dernier *commit*, mais garder les changements effectués dans votre système de fichiers :
```shell
git reset HEAD~
```
#### Défaire les deux derniers *commits*, et ajouter leurs changements à l'index (dans la zone de stage) :
```shell
git reset --soft HEAD~2
```
#### Enlever tout les changements qui n'ont pas été *commit*, qu'ils soient dans la *zone de stage* ou non (pour enlever seulement les changements de la *zone de stage*, utiliser `git checkout`) :
```shell
git reset --hard
```
#### Réinitialiser le dépôt à un commit spécifique en retirant tout les changements (ceci inclus les changements dans des commits entre la *tête* et le *commit* spécifié !) :
```shell
git reset --hard {{commit}}
```
{% endraw %}