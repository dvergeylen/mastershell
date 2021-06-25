---
layout: default
title: "git archive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-archive">
  <a href="/fr/common/git-archive.html">git archive</a> <a href="#git-archive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crée une archive de fichiers depuis un branche donnée.
> Plus d'informations : <https://git-scm.com/docs/git-archive>.

#### Crée une archive `.tar` avec le contenu de la HEAD et l'affiche sur la sortie standard :
```shell
git archive --verbose HEAD
```
#### Crée une archive `.zip` avec le contenu de la HEAD et l'affiche sur la sortie standard :
```shell
git archive --verbose --format=zip HEAD
```
#### Pareil que ci-dessus mais écrit dans l'archive spécifiée :
```shell
git archive --verbose --output={{chemin/vers/fichier.zip}} HEAD
```
#### Crée une archive depuis le dernier commit de la branche spécifiée :
```shell
git archive --output={{chemin/vers/fichier.tar}} {{nom_de_branche}}
```
#### Crée une archive avec le contenu d'un répertoire donné :
```shell
git archive --output={{chemin/vers/fichier.tar}} HEAD:{{chemin/vers/repertoire}}
```
#### Ajoutez un chemin d'accès à chaque fichier pour l'archiver dans un répertoire spécifique :
```shell
git archive --output={{chemin/vers/fichier.tar}} --prefix={{chemin/vers/cible}}/ HEAD
```
{% endraw %}