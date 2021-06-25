---
layout: default
title: "git format-patch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-format-patch">
  <a href="/fr/common/git-format-patch.html">git format-patch</a> <a href="#git-format-patch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Préparer des fichiers de correctifs, utiles pour les envoyer par courriel.
> Voir également `git am`, qui peut appliquer des fichiers de correctifs générés.
> Plus d'informations : <https://git-scm.com/docs/git-format-patch>.

#### Créer un fichier de correctif `.patch` nommé automatiquement pour tout les commits non poussés :
```shell
git format-patch {{origin}}
```
#### Créer un fichier correctif `.patch` pour les changements entre 2 révisions :
```shell
git format-patch {{revision_1}}..{{revision_2}}
```
#### Créer un fichier correctif `.patch` pour les 3 derniers commits :
```shell
git format-patch -{{3}}
```
{% endraw %}