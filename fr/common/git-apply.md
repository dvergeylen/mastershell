---
layout: default
title: "git apply"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-apply">
  <a href="/fr/common/git-apply.html">git apply</a> <a href="#git-apply"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Applique un correctif à un fichier et/ou à l index.
> Plus d'informations : <https://git-scm.com/docs/git-apply>.

#### Afficher les messages à propos des fichiers corrigés :
```shell
git apply --verbose {{chemin/vers/fichier}}
```
#### Applique le correctif et ajoute les fichiers à l index :
```shell
git apply --index {{chemin/vers/fichier}}
```
#### Applique un correctif depuis une source distante :
```shell
curl {{https://example.com/file.patch}} | git apply
```
#### Affiche les différences résultantes et applique le correctif :
```shell
git apply --stat --apply {{chemin/vers/fichier}}
```
#### Applique le correctif en ordre inverse :
```shell
git apply --reverse {{chemin/vers/fichier}}
```
#### Stocke le résultat du correctif dans l'index sans modifier la branche courante :
```shell
git apply --cache {{chemin/vers/fichier}}
```
{% endraw %}