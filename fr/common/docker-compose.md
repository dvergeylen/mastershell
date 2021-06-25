---
layout: default
title: "docker-compose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-compose">
  <a href="/fr/common/docker-compose.html">docker-compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exécute et gère des applications au travers de plusieurs conteneurs Docker.
> Plus d'informations : <https://docs.docker.com/compose/reference/overview/>.

#### Liste tous les conteneurs en cours d'exécution :
```shell
docker-compose ps
```
#### Crée et démarre en arrière-plan tous les conteneurs décrits dans le fichier `docker-compose.yml` du répertoire courant :
```shell
docker-compose up -d
```
#### Démarre tous les conteneurs après les avoir recréés si nécessaire :
```shell
docker-compose up --build
```
#### Démarre tous les conteneurs spécifiés dans un fichier compose alternatif :
```shell
docker-compose --file {{chemin/vers/fichier}} up
```
#### Arrête tous les conteneurs en cours d'exécution :
```shell
docker-compose stop
```
#### Arrête et supprime tous les conteneurs, réseaux, images et volumes :
```shell
docker-compose down --rmi all --volumes
```
#### Affiche et suit la journalisation de tous les conteneurs :
```shell
docker-compose logs --follow
```
#### Affiche et suit la journalisation pour un conteneurs spécifique :
```shell
docker-compose logs --follow {{nom_container}}
```
{% endraw %}