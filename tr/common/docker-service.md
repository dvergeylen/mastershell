---
layout: default
title: "docker service"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-service">
  <a href="/tr/common/docker-service.html">docker service</a> <a href="#docker-service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir docker daemon'unun üzerindeki servisleri yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/service/>.

#### Bir docker daeomon'unun üzerindeki servisleri listele:
```shell
docker service ls
```
#### Yeni bir servis yarat:
```shell
docker service create --name {{servis_ismi}} {{imge}}:{{etiket}}
```
#### Boşluk ile ayrılmış bir servis listesinin detaylı bilgisini görüntüle:
```shell
docker service inspect {{servis_ismi|ID}}
```
#### Boşluk ile ayrılmış bir servis listesinin görevlerini sırala:
```shell
docker service ps {{servis_ismi|ID}}
```
#### Boşluk ile ayrılmış bir servis listesi için belirli bir replika miktarına yüksel:
```shell
docker service scale {{servis_ismi}}={{replika_miktarı}}
```
#### Boşluk ile ayrılmış bir servis listesini sil:
```shell
docker service rm {{servis_ismi|ID}}
```
{% endraw %}