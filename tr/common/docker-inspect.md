---
layout: default
title: "docker inspect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-inspect">
  <a href="/tr/common/docker-inspect.html">docker inspect</a> <a href="#docker-inspect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker objelerinde bulunan düşük seviye bilgiyi gösterir.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/inspect/>.

#### Yardım içeriğini göster:
```shell
docker inspect
```
#### Bir konteyner, imge veya hacim ile ilgili bilgiyi ismini veya ID'sini girerek görüntüle:
```shell
docker inspect {{konteyner|imge|ID}}
```
#### Bir konteynerin IP adresini görüntüle:
```shell
docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' {{konteyner}}
```
#### Konteynerin log dosyasının yolunu görüntüle:
```shell
docker inspect --format='{{.LogPath}}' {{konteyner}}
```
#### Konteynerin imge ismini görüntüle:
```shell
docker inspect --format='{{.Config.Image}}' {{konteyner}}
```
#### Konfigürasyon bilgisini JSON olarak görüntüle:
```shell
docker inspect --format='{{json .Config}}' {{konteyner}}
```
#### Tüm port limanlayıcıları görüntüle:
```shell
docker inspect --format='{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -> {{(index $conf 0).HostPort}} {{end}}' {{konteyner}}
```
{% endraw %}