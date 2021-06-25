---
layout: default
title: "pip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pip">
  <a href="/fr/common/pip.html">pip</a> <a href="#pip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestionnaire des paquets pour Python.
> Plus d'informations : <https://pip.pypa.io>.

#### Installe un paquet :
```shell
pip install {{paquet}}
```
#### Installe une version particulière d'un paquet :
```shell
pip install {{paquet}}=={{version}}
```
#### Met à jour un paquet :
```shell
pip install -U {{paquet}}
```
#### Désinstalle un paquet :
```shell
pip uninstall {{paquet}}
```
#### Sauvegarde une liste des paquets installés :
```shell
pip freeze > {{requirements.txt}}
```
#### Installe des paquets à partir d'un fichier :
```shell
pip install -r {{requirements.txt}}
```
#### Affiche les informations d'un paquet installé :
```shell
pip show {{paquet}}
```
{% endraw %}