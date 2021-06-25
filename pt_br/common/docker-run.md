---
layout: default
title: "docker run"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-run">
  <a href="/pt_br/common/docker-run.html">docker run</a> <a href="#docker-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executa um comando em um novo container Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/run/>.

#### Executa um comando em um novo container de uma imagem tagueada:
```shell
docker run {{imagem:tag}} {{comando}}
```
#### Executa um comando em um novo container em background e exibe o ID:
```shell
docker run -d {{image}} {{command}}
```
#### Executa um comando em um novo container que será removido após a execução em um modo interativo e com um terminal TTY:
```shell
docker run --rm -it {{image}} {{command}}
```
#### Executa um comando em um novo container com variáveis de ambiente:
```shell
docker run -e '{{variável}}={{valor}}' -e {{variável}} {{imagem}} {{comando}}
```
#### Executa um comando em um novo container montando volumes nos caminhos específicos:
```shell
docker run -v {{caminho/no/host_local}}:{{caminho/no/container}} {{imagem}} {{comando}}
```
#### Executa um comando em um novo container e abre as portas para acesso:
```shell
docker run -p {{porta_do_host_local}}:{{porta_do_container}} {{imagem}} {{comando}}
```
{% endraw %}