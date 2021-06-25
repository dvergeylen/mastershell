---
layout: default
title: "docker logs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-logs">
  <a href="/pt_br/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe os logs dos containers.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/logs>.

#### Exibe logs de um container:
```shell
docker logs {{nome_do_container}}
```
#### Exibe logs de um container e segue exibindo:
```shell
docker logs -f {{nome_do_container}}
```
#### Exibe as últimas 5 linhas:
```shell
docker logs {{nome_do_container}} --tail {{5}}
```
#### Exibe logs e adiciona a informação de hora ao log:
```shell
docker logs -t {{nome_do_container}}
```
#### Exibe logs até um certo ponto no tempo de execução do container (por exemplo: 23m, 10s, 2013-01-02T13:23:37):
```shell
docker logs {{nome_do_container}} --until {{tempo}}
```
{% endraw %}