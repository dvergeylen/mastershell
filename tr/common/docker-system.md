---
layout: default
title: "docker system"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-system">
  <a href="/tr/common/docker-system.html">docker system</a> <a href="#docker-system"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker verilerini yönet ve sistem bilgisi görüntüle.
> More information: <https://docs.docker.com/engine/reference/commandline/system/>.

#### Yardım göster:
```shell
docker system
```
#### Docker disk kullanımını göster:
```shell
docker system df
```
#### Disk kullanımı üzerine detaylı bilgi göster:
```shell
docker system df --verbose
```
#### Kullanılmayan veriyi sil:
```shell
docker system prune
```
#### Kullanılmayan ve geçmişte birden çok kez oluşturulan veriyi sil:
```shell
docker system prune --filter="until={{saat}}h{{dakika}}m"
```
#### Docker deamon'dan tam-zamanlı eylemleri görüntüle:
```shell
docker system events
```
#### Geçerli JSON satırları olarak yayınlanan konteynerleden tam-zamanlı eylemleri göster:
```shell
docker system events --filter 'type=container' --format '{{json .}}'
```
#### Sistem bilgisi göster:
```shell
docker system info
```
{% endraw %}