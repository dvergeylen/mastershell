---
layout: default
title: "chmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chmod">
  <a href="/fr/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modifie les droits d'accès d'un fichier ou d'un répertoire.
> Plus d'informations : <https://www.gnu.org/software/coreutils/chmod>.

#### Donne les droits d'e[x]écution à l'[u]tilisateur auquel le fichier appartient :
```shell
chmod u+x {{fichier}}
```
#### Donne à l'utilisateur les droits de lecture (r) et d'écriture (w) sur un fichier/répertoire :
```shell
chmod u+rw {{fichier_ou_repertoire}}
```
#### Enlève les droits d'exécution pour le [g]roupe :
```shell
chmod g-x {{fichier}}
```
#### Donne à tous (a) les utilisateurs les droits de lecture et d'exécution :
```shell
chmod a+rx {{fichier}}
```
#### Donne aux autres utilisateurs (qui sont dans un autre groupe) les mêmes droits que ceux du groupe propriétaire :
```shell
chmod o=g {{fichier}}
```
#### Retire tous les droits aux autres (o) utilisateurs :
```shell
chmod o= {{fichier}}
```
#### Modifie les permissions récursivement en donnant aux membres du groupe et aux autres utilisateurs le droit d'écriture :
```shell
chmod -R g+w,o+w {{repertoire}}
```
{% endraw %}