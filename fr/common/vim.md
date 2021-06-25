---
layout: default
title: "vim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vim">
  <a href="/fr/common/vim.html">vim</a> <a href="#vim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vim (Vi IMproved), un éditeur de texte en ligne de commandes, fournit plusieurs modes pour différentes manipulations de texte.
> Pressez `i` pour passer en mode édition. `<Esc>` revient au mode normal, qui ne permet pas l insertion de code.
> Plus d'informations : <https://www.vim.org>.

#### Ouvrir un fichier :
```shell
vim {{chemin/vers/fichier}}
```
#### consulter le manuel utilisateur :
```shell
:help<Entrée>
```
#### Sauvegarder et fermer :
```shell
:wq<Entrée>
```
#### Ouvrir un fichier à une ligne spécifiée :
```shell
vim +{{numero_ligne}} {{chemin/vers/fichier}}
```
#### Annuler la dernière opération :
```shell
u
```
#### Rechercher un motif dans un fichier (appuyez `n`/`N` pour aller à la prochaine / précédente occurrence) :
```shell
/{{motif_recherché}}<Entrée>
```
#### Effectuer une substitution par expression régulière dans tout le fichier :
```shell
:%s/{{motif}}/{{remplacement}}/g<Entrée>
```
#### Afficher les numéros de ligne :
```shell
:set nu<Entrée>
```
{% endraw %}