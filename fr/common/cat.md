---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/fr/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche et concatène le contenu d'un ou plusieurs fichiers.
> Plus d'informations : <https://www.gnu.org/software/coreutils/cat>.

#### Affiche le contenu d'un fichier sur la sortie standard :
```shell
cat {{fichier}}
```
#### Concatène le contenu de plusieurs fichiers vers le fichier de destination :
```shell
cat {{fichier1}} {{fichier2}} > {{fichier_de_destination}}
```
#### Ajoute le contenu d'un ficher à la fin du fichier de destination :
```shell
cat {{fichier1}} {{fichier2}} >> {{fichier_de_destination}}
```
#### Numérote toutes les lignes affichées :
```shell
cat -n {{fichier}}
```
#### Affiche les caractères non-imprimables ainsi que les caractères d'espacement (en utilisant le préfixe `M-` si non-ASCII) :
```shell
cat -v -t -e {{fichier}}
```
{% endraw %}