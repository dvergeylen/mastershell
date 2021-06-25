---
layout: default
title: "basename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="basename">
  <a href="/fr/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retourne la portion ne contenant pas de dossiers d'un chemin complet.
> Plus d'informations : <https://www.gnu.org/software/coreutils/basename>.

#### N'afficher que le nom du fichier depuis un chemin :
```shell
basename {{chemin/vers/fichier}}
```
#### N'afficher que le nom du dernier répertoire depuis un chemin :
```shell
basename {{chemin/vers/répertoire/}}
```
#### N'afficher que le nom du fichier depuis un chemin, en ôtant un préfixe donné :
```shell
basename {{chemin/vers/fichier}} {{suffixe}}
```
{% endraw %}