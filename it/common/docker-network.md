---
layout: default
title: "docker network"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-network">
  <a href="/it/common/docker-network.html">docker network</a> <a href="#docker-network"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea e gestisci reti docker.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/network/>.

#### Elenca le reti disponibili configurate sul docker daemon:
```shell
docker network ls
```
#### Crea una rete definita da un utente:
```shell
docker network create --driver {{nome_del_driver}} {{nome_rete}}
```
#### Mostra informazioni dettagliate su una lista di reti (separata da spazi):
```shell
docker network inspect {{nome_rete_1 nome_rete_2}}
```
#### Connetti un container ad una rete usando il suo nome o ID:
```shell
docker network connect {{nome_rete}} {{nome_container|ID}}
```
#### Disconnetti un container da una rete:
```shell
docker network disconnect {{nome_rete}} {{nome_container|ID}}
```
#### Elimina le reti inutilizzate (non referenziate da alcun container):
```shell
docker network prune
```
#### Elimina una lista di reti (separata da spazi) inutilizzate:
```shell
docker network rm {{nome_rete_1 nome_rete_2}}
```
{% endraw %}