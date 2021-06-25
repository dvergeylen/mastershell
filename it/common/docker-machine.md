---
layout: default
title: "docker-machine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-machine">
  <a href="/it/common/docker-machine.html">docker-machine</a> <a href="#docker-machine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea e gestisci macchine che utilizzano Docker.
> Maggiori informazioni: <https://docs.docker.com/machine/reference/>.

#### Elenca macchine Docker in esecuzione:
```shell
docker-machine ls
```
#### Crea una nuova macchina Docker con uno specifico nome:
```shell
docker-machine create {{nome}}
```
#### Mostra lo stato di una macchina:
```shell
docker-machine status {{nome}}
```
#### Avvia una macchina:
```shell
docker-machine start {{nome}}
```
#### Arresta una macchina:
```shell
docker-machine stop {{nome}}
```
#### Ispeziona le informazioni su di una macchina:
```shell
docker-machine inspect {{nome}}
```
{% endraw %}