---
layout: default
title: "docker images"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-images">
  <a href="/pt_br/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia imagens Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/images/>.

#### Lista todas as imagens Docker:
```shell
docker images
```
#### Lista todas as imagens Docker incluíndo imagens intermedirárias:
```shell
docker images --all
```
#### Lista no modo silencioso (somente IDs numéricos):
```shell
docker images --quiet
```
#### Lista todas as imagens Docker não usadas por nenhum container:
```shell
docker images --filter dangling=true
```
#### Lista imagens que contenham um substring no seu nome:
```shell
docker images "{{*nome*}}"
```
{% endraw %}