---
layout: default
title: "git bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bundle">
  <a href="/fr/common/git-bundle.html">git bundle</a> <a href="#git-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Empaquetez des objets et des références dans une archive.
> Plus d'informations : <https://git-scm.com/docs/git-bundle>.

#### Empaquetez tout les objets et les références d'une branche spécifiée :
```shell
git bundle create {{chemin/vers/fichier.bundle}} {{nom_de_branche}}
```
#### Crée un empaquetage de tout les fichiers de toutes les branches :
```shell
git bundle create {{chemin/vers/fichier.bundle}} --all
```
#### Crée un empaquetage des 5 derniers commits de la branche courante :
```shell
git bundle create {{chemin/vers/fichier.bundle}} -{{5}} {{HEAD}}
```
#### Crée un empaquetage des 7 derniers jours :
```shell
git bundle create {{chemin/vers/fichier.bundle}} --since={{7.days}} {{HEAD}}
```
#### Vérifie qu'un empaquetage est valide et peut être appliqué à la branche courante :
```shell
git bundle verify {{chemin/vers/fichier.bundle}}
```
#### Affiche sur la sortie standard la liste des références contenues dans un empaquetage :
```shell
git bundle unbundle {{chemin/vers/fichier.bundle}}
```
#### Extraire une branche spécifique d'un fichier de bundle dans le référentiel actuel :
```shell
git pull {{chemin/vers/fichier.bundle}} {{nom_de_branche}}
```
{% endraw %}