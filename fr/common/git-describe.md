---
layout: default
title: "git describe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-describe">
  <a href="/fr/common/git-describe.html">git describe</a> <a href="#git-describe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Créer un nom unique et lisible pour un objet à partir d'une référence disponible.
> Plus d'informations : <https://git-scm.com/docs/git-describe>.

#### Créer un nom unique pour le commit courant (le nom contient le tag le plus récent, le nombre de commits additionnels, et l'empreinte abrégée du commit) :
```shell
git describe
```
#### Créer un nom avec une empreinte de commit de 4 caractères :
```shell
git describe --abbrev={{4}}
```
#### Générer un nom avec le chemin complet du tag :
```shell
git describe --all
```
#### Décrire un tag Git :
```shell
git describe {{v1.0.0}}
```
#### Créer un nom pour le dernier commit d'une branche donnée :
```shell
git describe {{nom_de_branche}}
```
{% endraw %}