---
layout: default
title: "pip3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pip3">
  <a href="/fr/common/pip3.html">pip3</a> <a href="#pip3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestionnaire des paquets pour Python.
> Plus d'informations : <https://pip.pypa.io>.

#### Recherche un paquet :
```shell
pip3 search {{paquet}}
```
#### Installe un paquet :
```shell
pip3 install {{paquet}}
```
#### Installe une version particulière d'un paquet :
```shell
pip3 install {{paquet}}=={{version}}
```
#### Met à jour un paquet :
```shell
pip3 install --upgrade {{paquet}}
```
#### Désinstalle un paquet :
```shell
pip3 uninstall {{paquet}}
```
#### Sauvegarde une liste des paquets installés :
```shell
pip3 freeze > {{requirements.txt}}
```
#### Installe des paquets à partir d'un fichier :
```shell
pip3 install --requirement {{requirements.txt}}
```
#### Affiche les informations d'un paquet installé :
```shell
pip3 show {{paquet}}
```
{% endraw %}