---
layout: default
title: "fdupes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdupes">
  <a href="/fr/common/fdupes.html">fdupes</a> <a href="#fdupes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trouve les fichiers dupliqués dans les dossiers donnés.
> Plus d'informations : <https://github.com/adrianlopezroche/fdupes>.

#### Chercher dans un dossier :
```shell
fdupes {{dossier}}
```
#### Chercher dans plusieurs dossiers :
```shell
fdupes {{dossier1}} {{dossier2}}
```
#### Chercher dans un dossier récursivement :
```shell
fdupes -r {{dossier}}
```
#### Chercher dans plusieurs dossiers dont un récursivement :
```shell
fdupes {{dossier1}} -R {{dossier2}}
```
#### Chercher récursivement les dupliqués et demander les fichiers à conserver, supprimant les autres :
```shell
fdupes -rd {{dossier}}
```
#### Chercher récursivement et supprimer les dupliqués automatiquement :
```shell
fdupes -rdN {{dossier}}
```
{% endraw %}