---
layout: default
title: "tput"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tput">
  <a href="/fr/common/tput.html">tput</a> <a href="#tput"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Accède et modifie les paramètres du terminal.

#### Déplace le curseur à un endroit donné sur l'écran :
```shell
tput cup {{coordonnée_y}} {{coordonnée_x}}
```
#### Règle la couleur de l'avant-plan (af) ou de l'arrière-plan (ab) :
```shell
tput {{setaf|setab}} {{code_de_couleur_ANSI}}
```
#### Affiche le numéro de colonnes, de rangées, ou de couleurs :
```shell
tput {{cols|lines|colors}}
```
#### Active la sonnerie du terminal :
```shell
tput bel
```
#### Réinitialise tous les attributs du terminal :
```shell
tput sgr0
```
#### Active ou désactive le retour automatique à la ligne :
```shell
tput {{smam|rmam}}
```
{% endraw %}