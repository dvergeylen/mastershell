---
layout: default
title: "docker stats"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-stats">
  <a href="/tr/common/docker-stats.html">docker stats</a> <a href="#docker-stats"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konteynerler için kaynak kullanım istatistiklerinin canlı yayınını görüntüle.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/stats/>.

#### Çalışan tüm konteynerlerin aynak kullanım istatistiklerinin canlı yayınını görüntüle:
```shell
docker stats
```
#### Boşluk ile ayrılmış bir listedeki konteynerlerin canlı yayınını görüntüle:
```shell
docker stats {{container_ismi}}
```
#### Konteyner'in CPU kullanım yüzdesini göstermek için sütun formatını değiştir:
```shell
docker stats --format "{{.Name}}:\t{{.CPUPerc}}"
```
#### Tüm (çalışan veya durmuş) konteynerler için istatistikleri görüntüle:
```shell
docker stats --all
```
#### İstatistikleri canlı yayınlamayı durdur ve yalnızca mevcut durumdaki istatistikleri görüntüle:
```shell
docker stats --no-stream
```
{% endraw %}