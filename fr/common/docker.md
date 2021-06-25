---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/fr/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestion des conteneurs et des images Docker.
> Plus d'informations : <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Liste les conteneurs Docker en cours d'exécution :
```shell
docker ps
```
#### Liste tous les conteneurs Docker (en cours d'exécution ou arrêtés) :
```shell
docker ps -a
```
#### Démarre un conteneur à partir d'une image, avec un nom personnalisé :
```shell
docker run --name {{nom_conteneur}} {{image}}
```
#### Démarre ou arrête un conteneur existant :
```shell
docker {{start|stop}} {{nom_conteneur}}
```
#### Télécharge une image depuis un registre Docker :
```shell
docker pull {{image}}
```
#### Ouvre un shell dans un conteneur déjà en cours d'exécution :
```shell
docker exec -it {{nom_conteneur}} {{sh}}
```
#### Supprime un conteneur arrêté :
```shell
docker rm {{nom_conteneur}}
```
#### Récupère et suit les journaux de message d'un conteneur :
```shell
docker logs -f {{nom_conteneur}}
```
{% endraw %}