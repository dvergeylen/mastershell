---
layout: default
title: "docker container"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-container">
  <a href="/it/common/docker-container.html">docker container</a> <a href="#docker-container"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci container Docker.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/container/>.

#### Elenca i container Docker attualmente in esecuzione:
```shell
docker container ls
```
#### Avvia uno o più container fermi:
```shell
docker container start {{nome_container1}} {{nome_container2}}
```
#### Termina uno o più container in esecuzione:
```shell
docker container kill {{nome_container}}
```
#### Ferma uno o più container in esecuzione:
```shell
docker container stop {{nome_container}}
```
#### Sospendi tutti i processi dentro uno o più container:
```shell
docker container pause {{nome_container}}
```
#### Mostra informazioni dettagliate su uno o più container:
```shell
docker container inspect {{nome_container}}
```
#### Esporta il filesystem di un container come archivio tar:
```shell
docker container export {{nome_container}}
```
#### Crea una nuova immagine dai cambiamenti di un container:
```shell
docker container commit {{nome_container}}
```
{% endraw %}