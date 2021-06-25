---
layout: default
title: "docker ps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-ps">
  <a href="/pt_br/common/docker-ps.html">docker ps</a> <a href="#docker-ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lista os containers Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/ps/>.

#### Lista containers docker em execução:
```shell
docker ps
```
#### Lista todos containers docker (em execução e parados):
```shell
docker ps --all
```
#### Lista os últimos containers criados (incluí todos os estados):
```shell
docker ps --latest
```
#### Filtra os containers que contém uma substring no seu nome:
```shell
docker ps --filter="name={{nome}}"
```
#### Filtra todos os containers que possuem uma imagem antepassada:
```shell
docker ps --filter "ancestor={{imagem}}:{{tag}}"
```
#### Filtra containers que tenha o código de saída:
```shell
docker ps --all --filter="exited={{código}}"
```
#### Filtra containers por estado (criado, execução, removendo, pausado, finalizado e morto):
```shell
docker ps --filter="status={{estado}}"
```
#### Filtra containers que contenham um volume específico ou montado em um caminho específico:
```shell
docker ps --filter="volume={{caminho/para/diretório}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"
```
{% endraw %}