---
layout: default
title: "pipenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pipenv">
  <a href="/fr/common/pipenv.html">pipenv</a> <a href="#pipenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Workflow de développement simple et unifié pour Python.
> Gère les paquets et l'environnement virtuel d'un projet.
> Plus d'informations : <https://pypi.org/project/pipenv>.

#### Crée un nouveau projet :
```shell
pipenv
```
#### Crée un nouveau projet à l'aide de Python 3 :
```shell
pipenv --three
```
#### Installe un paquet :
```shell
pipenv install {{paquet}}
```
#### Installe toutes les dépendances d'un projet :
```shell
pipenv install
```
#### Installe toutes les dépendances d'un projet (y compris les paquets de développement) :
```shell
pipenv install --dev
```
#### Désinstalle un paquet :
```shell
pipenv uninstall {{paquet}}
```
#### Démarre une session de commandes dans l'environnement virtuel :
```shell
pipenv shell
```
#### Génère un `requirements.txt` (une liste de dépendances) pour un projet :
```shell
pipenv lock --requirements
```
{% endraw %}