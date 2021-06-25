---
layout: default
title: "docker start"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-start">
  <a href="/tr/common/docker-start.html">docker start</a> <a href="#docker-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla durmuş konteyneri başlar.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/start/>.

#### Yardım göster:
```shell
docker start
```
#### Bir docker konteynerini başlat:
```shell
docker start {{konteyner}}
```
#### Bir konteyneri, ona stdout ile stderr'i ekleyerek ve sinyaller göndererek başlat:
```shell
docker start --attach {{konteyner}}
```
#### Bir veya daha fazla boşlukla ayrılarak belirtilmiş konteynerleri başlar:
```shell
docker start {{konteyner(ler)}}
```
{% endraw %}