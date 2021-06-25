---
layout: default
title: "docker swarm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-swarm">
  <a href="/tr/common/docker-swarm.html">docker swarm</a> <a href="#docker-swarm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir konteyner orkestrasyon aracı.
> Daha fazla bilgi için: <https://docs.docker.com/engine/swarm/>.

#### Bir bataklık dizisi oluştur:
```shell
docker swarm init
```
#### Bir yönetici veya işçiye takılmak için token göster:
```shell
docker swarm join-token {{işçi|yönetici}}
```
#### Diziye yeni bir düğüm ekle:
```shell
docker swarm join --token {{token}} {{manager_node_url:2377}}
```
#### Bir işçiyi bataklıktan sil (işçi düğümünün içinde çalıştır):
```shell
docker swarm leave
```
#### Mevcut CA sertifikasını PEM formatında görüntüle:
```shell
docker swarm ca
```
#### Mevcut CA sertifikasını döndür ve yeni sertifikayı görüntüle:
```shell
docker swarm ca --rotate
```
#### Düğüm sertifikaları için geçerli periyodu değiştir:
```shell
docker swarm update --cert-expiry {{saat}}h{{dakika}}m{{saniye}}s
```
{% endraw %}