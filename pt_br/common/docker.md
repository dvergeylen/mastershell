---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/pt_br/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de containers e imagens Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Listar os containers Docker que se encontram em execução:
```shell
docker ps
```
#### Listar todos os containers Docker:
```shell
docker ps -a
```
#### Inicializar um container com um nome personalizado a partir de uma imagem:
```shell
docker run --name {{nome_container}} {{imagem}}
```
#### Começar ou parar um container existente:
```shell
docker {{start|stop}} {{nome_container}}
```
#### Extrair uma imagem a partir de um Docker Registry:
```shell
docker pull {{imagem}}
```
#### Abrir um terminal dentro de um container em execução:
```shell
docker exec -it {{nome_container}} {{sh}}
```
#### Remover um container parado:
```shell
docker rm {{nome_container}}
```
#### Obter e acompanhar o histórico de um container:
```shell
docker logs -f {{nome_container}}
```
{% endraw %}