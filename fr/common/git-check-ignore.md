---
layout: default
title: "git check-ignore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-check-ignore">
  <a href="/fr/common/git-check-ignore.html">git check-ignore</a> <a href="#git-check-ignore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analyser et déboguer les fichiers ignorés / exclus (".gitignore") de Git.
> Plus d'informations : <https://git-scm.com/docs/git-check-ignore>.

#### Vérifie qu'un fichier ou répertoire est ignoré :
```shell
git check-ignore {{chemin/vers/fichier_ou_répertoire}}
```
#### Vérifie que plusieurs fichiers ou répertoires sont ignorés :
```shell
git check-ignore {{chemin/vers/fichier}} {{chemin/vers/répertoire}}
```
#### Utilisez des chemins d'accès, un par ligne, de stdin :
```shell
git check-ignore --stdin < {{chemin/vers/fichier_annexe}}
```
#### Ne pas vérifier l'index (utilisé pour déboguer pourquoi les chemins ont été suivis et non ignorés) :
```shell
git check-ignore --no-index {{chemin/vers/fichiers_ou_répertoires}}
```
#### Inclure les détails pour chaque occurrence dans le chemin :
```shell
git check-ignore --verbose {{chemin/vers/fichiers_ou_répertoires}}
```
{% endraw %}