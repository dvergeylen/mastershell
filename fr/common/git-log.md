---
layout: default
title: "git log"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-log">
  <a href="/fr/common/git-log.html">git log</a> <a href="#git-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Afficher un historique de commits.
> Plus d'informations : <https://git-scm.com/docs/git-log>.

#### Afficher la séquence de commits à partir de l'actuel, dans l'ordre chronologique inverse du dépôt Git dans le répertoire de travail actuel :
```shell
git log
```
#### Afficher l'historique de fichiers ou répertoires en particulier :
```shell
git log -p {{chemin/vers/fichier_ou_repertoire}}
```
#### Afficher la liste des fichiers modifiés pour chaque commit :
```shell
git log --stat
```
#### Afficher un graphique des commits dans la branche actuelle en utilisant uniquement la première ligne de chaque message de commit :
```shell
git log --oneline --graph
```
#### Afficher un graphique de tout les commits, tags et branches dans le dépôt entier :
```shell
git log --oneline --decorate --all --graph
```
#### Afficher uniquement les commits dont le message contient la chaine (non sensible à la casse) :
```shell
git log -i --grep {{chaine_recherché}}
```
#### Afficher les N derniers commits d'un utilisateur :
```shell
git log -n {{number}} --author={{author}}
```
#### Afficher les commits entre deux dates :
```shell
git log --before={{date}} --after={{date}}
```
{% endraw %}