---
layout: default
title: "docker-compose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-compose">
  <a href="/it/common/docker-compose.html">docker-compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui e gestisci applicazioni Docker composte da più container.
> Maggiori informazioni: <https://docs.docker.com/compose/reference/overview/>.

#### Elenca i container in esecuzione:
```shell
docker-compose ps
```
#### Crea ed avvia tutti i container in background utilizzando il file `docker-compose.yml` nella directory corrente:
```shell
docker-compose up -d
```
#### Avvia tutti i container, buildandoli di nuovo se necessario:
```shell
docker-compose up --build
```
#### Avvia tutti i container utilizzando un file compose alternativo:
```shell
docker-compose --file {{percorso/a/file}} up
```
#### Ferma tutti i container in esecuzione:
```shell
docker-compose stop
```
#### Ferma e rimuovi tutti i container, reti, immagini e volumi:
```shell
docker-compose down
```
#### Segui i log di tutti i container:
```shell
docker-compose logs --follow
```
#### Segui i log di un container specifico:
```shell
docker-compose logs --follow {{nome_container}}
```
{% endraw %}