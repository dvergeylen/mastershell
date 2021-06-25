---
layout: default
title: "docker logs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-logs">
  <a href="/it/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra i log di un container.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/logs>.

#### Mostra i log di un container:
```shell
docker logs {{nome_container}}
```
#### Segui i log di un container:
```shell
docker logs -f {{nome_container}}
```
#### Mostra le ultime 5 righe:
```shell
docker logs {{nome_container}} --tail {{5}}
```
#### Mostra i log mettendo un timestamp in coda:
```shell
docker logs -t {{nome_container}}
```
#### Mostra i log avvenuti prima di un dato momento nell'esecuzione del container (ad esempio, 23m, 10s, 2013-01-02T13:23:37):
```shell
docker logs {{nome_container}} --until {{momento}}
```
{% endraw %}