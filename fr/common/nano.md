---
layout: default
title: "nano"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nano">
  <a href="/fr/common/nano.html">nano</a> <a href="#nano"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Éditeur de texte simple et convivial. C'est un clone libre et amélioré de Pico.
> Plus d'informations : <https://nano-editor.org>.

#### Ouvre un fichier :
```shell
nano {{chemin/vers/fichier}}
```
#### Ouvre un fichier en positionnant le curseur à une rangée et colonne donnée :
```shell
nano +{{ligne}},{{colonne}} {{chemin/vers/fichier}}
```
#### Active le défilement fluide :
```shell
nano -S {{fichier}}
```
#### Indente les nouvelles lignes à la même indentation que les lignes précédentes :
```shell
nano -i {{fichier}}
```
#### Avant la modification, sauvegarde le fichier actuel sous le format `{{nom_du_fichier_actuel}}~` :
```shell
nano -B {{fichier}}
```
{% endraw %}