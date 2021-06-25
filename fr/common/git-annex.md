---
layout: default
title: "git annex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-annex">
  <a href="/fr/common/git-annex.html">git annex</a> <a href="#git-annex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gérez les fichiers avec Git, sans archiver leur contenu.
> Lorsqu'un fichier est annexé, son contenu est déplacé dans un stockage clé-valeur et un lien symbolique est créé qui pointe vers le contenu.
> Plus d'informations : <https://git-annex.branchable.com>.

#### Aide :
```shell
git annex help
```
#### Initialise le dépôt :
```shell
git annex init
```
#### Ajoute un fichier :
```shell
git annex add {{chemin/vers/fichier_ou_repertoire}}
```
#### Affiche le statut courant d'un fichier ou répertoire :
```shell
git annex status {{chemin/vers/fichier_ou_repertoire}}
```
#### Synchronise un dépôt local avec un distant :
```shell
git annex {{distant}}
```
#### Récupère un fichier ou un répertoire :
```shell
git annex get {{chemin/vers/fichier_ou_repertoire}}
```
{% endraw %}