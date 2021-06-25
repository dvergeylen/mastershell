---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/it/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci container ed immagini Docker.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Elenca i container Docker attualmente in esecuzione:
```shell
docker ps
```
#### Elenca tutti i container Docker (in esecuzione e arrestati):
```shell
docker ps -a
```
#### Avvia un container da una immagine, con un nome personalizzato:
```shell
docker run --name {{nome_container}} {{immagine}}
```
#### Avvia o arresta un container esistente:
```shell
docker {{start|stop}} {{nome_container}}
```
#### Scarica (pull) un'immagine dal Docker registry:
```shell
docker pull {{image}}
```
#### Avvia una shell all'interno di un container in esecuzione:
```shell
docker exec -it {{nome_container}} {{sh}}
```
#### Rimuovi un container arrestato:
```shell
docker rm {{nome_container}}
```
#### Ottieni e visualizza i log di un container:
```shell
docker logs -f {{nome_container}}
```
{% endraw %}