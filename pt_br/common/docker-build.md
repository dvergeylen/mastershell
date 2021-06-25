---
layout: default
title: "docker build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-build">
  <a href="/pt_br/common/docker-build.html">docker build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cria uma imagem a partir de um Dockerfile.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/build/>.

#### Cria uma imagem docker usando o Dockerfile presente no diretório atual:
```shell
docker build .
```
#### Cria uma imagem docker usando o Dockerfile de uma URL específica:
```shell
docker build {{github.com/creack/docker-firefox}}
```
#### Cria uma imagem docker e cria uma tag para ela:
```shell
docker build --tag {{nome:tag}} .
```
#### Não usa o cache na criação da imagem:
```shell
docker build --no-cache --tag {{nome:tag}} .
```
#### Cria uma imagem docker usando um Dockerfile específico:
```shell
docker build --file {{Dockerfile}} .
```
#### Cria uma imagem docker utilizando variáveis customizadas para a criação de imagens:
```shell
docker build --build-arg {{PROXY_DO_HTTP=http://10.20.30.2:1234}} --build-arg {{PROXY_DO_FTP=http://40.50.60.5:4567}} .
```
{% endraw %}