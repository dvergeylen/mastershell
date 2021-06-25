---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/tr/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker konteyner ve imgelerini yönetir.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Şuan çalışan docker konteynerlerini listele:
```shell
docker ps
```
#### Tüm (çalışan veya duran) docker konteynerlerini listele:
```shell
docker ps -a
```
#### Bir imgeden özel bir isimle konteyner başlat:
```shell
docker run --name {{konteyner_ismi}} {{imge}}
```
#### Varolan bir konteyneri başlat veya durdur:
```shell
docker {{baslat|durdur}} {{konteyner_ismi}}
```
#### Bir docker kaydından imge çek:
```shell
docker pull {{imge}}
```
#### Halihazırda çalışan bir konteyner içinde komut istemcisi aç:
```shell
docker exec -it {{konteyner_ismi}} {{sh}}
```
#### Durmuş bir konteyneri sil:
```shell
docker rm {{konteyner_ismi}}
```
#### Bir konteynerin kaydını çek ve takip et:
```shell
docker logs -f {{konteyner_ismi}}
```
{% endraw %}