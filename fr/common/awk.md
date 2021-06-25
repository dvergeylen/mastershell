---
layout: default
title: "awk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="awk">
  <a href="/fr/common/awk.html">awk</a> <a href="#awk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Langage de programmation polyvalent pour travailler sur des fichiers.
> Plus d'informations : <https://github.com/onetrueawk/awk>.

#### Affiche la cinquième colonne (ou le champ) dans un fichier qui utilise des espaces comme séparateur :
```shell
awk '{print $5}' {{nom_de_fichier}}
```
#### Affiche la deuxième colonne dans des lignes contenant "quelque-chose" dans un fichier qui utilise des espaces comme séparateur :
```shell
awk '/{{quelque-chose}}/ {print $2}' {{nom_de_fichier}}
```
#### Affiche la dernière colonne de chaque ligne d'un fichier en utilisant une virgule (au lieu des espaces) comme séparateur :
```shell
awk -F ',' '{print $NF}' {{nom_de_fichier}}
```
#### Additionne les valeurs de la première colonne des lignes d'un fichier et affiche le total :
```shell
awk '{s+=$1} END {print s}' {{nom_de_fichier}}
```
#### Additionne les valeurs de la première colonne des lignes d'un fichier et affiche ces valeurs puis affiche le total :
```shell
awk '{s+=$1; print $1} END {print "--------"; print s}' {{nom_de_fichier}}
```
#### Affiche une ligne sur trois en partant de la première ligne :
```shell
awk 'NR%3==1' {{nom_de_fichier}}
```
#### Affiche les lignes dont la valeur de la colonne 10 vaut la valeur recherchée :
```shell
awk '($10 == valeur)'
```
#### Affiche les lignes dont la valeur de la colonne 10 est comprise entre un min et un max :
```shell
awk '($10 >= valeur_min && $10 <= valeur_max)'
```
{% endraw %}