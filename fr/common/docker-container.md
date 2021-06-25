---
layout: default
title: "docker container"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-container">
  <a href="/fr/common/docker-container.html">docker container</a> <a href="#docker-container"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gère les conteneurs Docker.
> Plus d'informations : <https://docs.docker.com/engine/reference/commandline/container/>.

#### Liste les conteneurs Dockers en cours d'exécution :
```shell
docker container ls
```
#### Démarre un ou plusieurs conteneur arrêtés :
```shell
docker container start {{nom_conteneur_1}} {{nom_conteneur_2}}
```
#### Tue un ou plusieurs conteneurs en cours d'exécution :
```shell
docker container kill {{nom_conteneur}}
```
#### Arrête un ou plusieurs conteneurs en cours d'exécution :
```shell
docker container stop {{nom_conteneur}}
```
#### Mets en pause tous les processus d'un ou plusieurs conteneurs :
```shell
docker container pause {{nom_conteneur}}
```
#### Affiche des informations détaillées sur un ou plusieurs conteneurs :
```shell
docker container inspect {{nom_conteneur}}
```
#### Exporte le système de fichiers d'un conteneur sous forme d'archive Tar :
```shell
docker container export {{nom_conteneur}}
```
#### Crée une nouvelle image à partir des changements d'un conteneur :
```shell
docker container commit {{nom_conteneur}}
```
{% endraw %}