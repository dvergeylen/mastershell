---
layout: default
title: "docker logs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-logs">
  <a href="/tr/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konteyner kaydını yazdırır.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/logs>.

#### Bir konteyner içindeki kayıtları yazdır:
```shell
docker logs {{konteyner_ismi}}
```
#### Kayıtları yazdır ve izle:
```shell
docker logs -f {{konteyner_ismi}}
```
#### Son 5 kaydı yazdır:
```shell
docker logs {{konteyner_ismi}} --tail {{5}}
```
#### Kayıtları yazdır ve zaman damgaları ile iliştir:
```shell
docker logs -t {{konteyner_ismi}}
```
#### Belli bir konteyner çalışma zamanındaki (i.e. 23m, 10s, 2013-01-02T13:23:37) kayıtları yazdır:
```shell
docker logs {{konteyner_ismi}} --until {{zaman}}
```
{% endraw %}