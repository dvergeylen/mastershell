---
layout: default
title: "clear"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clear">
  <a href="/fr/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Efface l'écran du terminal.
> Plus d'informations : <https://manned.org/clear>.

#### Effacer l'écran (identique à la séquence Contrôle-L sur une interface bash) :
```shell
clear
```
#### Effacer l'écran mais conserve le tampon de défilement du terminal :
```shell
clear -x
```
#### Indiquer le type de terminal à effacer (utilise par défaut la variable d'environnement `TERM`) :
```shell
clear -T {{type_de_terminal}}
```
#### Afficher la version de `ncurses` utilisée par `clear` :
```shell
clear -V
```
{% endraw %}