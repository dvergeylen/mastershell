---
layout: default
title: "ghdl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ghdl">
  <a href="/fr/common/ghdl.html">ghdl</a> <a href="#ghdl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simulateur à source ouvert pour le langage VHDL.
> Plus d'informations : <http://ghdl.free.fr>.

#### Analyse un fichier de source VHDL et génère un fichier objet :
```shell
ghdl -a {{fichier.vhdl}}
```
#### Élabore un design (où `{{design}}` est le nom d'une unité de configuration, d'entité, ou d'architecture) :
```shell
ghdl -e {{design}}
```
#### Exécute un design élaboré :
```shell
ghdl -r {{design}}
```
#### Exécute un design élaboré et sauvegarde la sortie à un fichier de forme d'onde :
```shell
ghdl -r {{design}} --wave={{sortie.ghw}}
```
#### Vérifie le syntaxe d'un fichier de source VHDL :
```shell
ghdl -s {{fichier.vhdl}}
```
#### Affiche l'aide générale :
```shell
ghdl --help
```
{% endraw %}