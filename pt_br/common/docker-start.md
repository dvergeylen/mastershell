---
layout: default
title: "docker start"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-start">
  <a href="/pt_br/common/docker-start.html">docker start</a> <a href="#docker-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inicia um ou mais containers parados.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/start/>.

#### Exibe a ajuda:
```shell
docker start
```
#### Inicia um container docker:
```shell
docker start {{container}}
```
#### Inicia um container, atachando ao terminal os sinais stdout e stderr e outros sinais:
```shell
docker start --attach {{container}}
```
#### Inicia um ou mais containers com ID separados por espaço:
```shell
docker start {{container(s)}}
```
{% endraw %}