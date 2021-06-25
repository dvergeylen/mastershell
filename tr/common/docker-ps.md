---
layout: default
title: "docker ps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-ps">
  <a href="/tr/common/docker-ps.html">docker ps</a> <a href="#docker-ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker konteynerlerini sırala.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/ps/>.

#### Halihazırda çalışan docker konteynerlerini listele:
```shell
docker ps
```
#### Tüm (durmuş veya çalışan) docker konteynerlerini listele:
```shell
docker ps --all
```
#### En son oluşturulan (durmuş veya çalışan) konteynerleri listele:
```shell
docker ps --latest
```
#### İsimlerinde belirtilen dizeleri içeren konteynerleri filtrele:
```shell
docker ps --filter="name={{isim}}"
```
#### Belirtilen imge ile akrabalık taşıyan konteynerleri filtrele:
```shell
docker ps --filter "ancestor={{imge}}:{{tag}}"
```
#### Konteynerleri çıkış durum koduna göre filtrele:
```shell
docker ps --all --filter="exited={{kod}}"
```
#### Konteynerleri mevcut durumlarına (oluşturulma, çalışma, silinme, durma, çıkma ve ölme) göre sırala:
```shell
docker ps --filter="status={{mevcut_durum}}"
```
#### Belirtilmiş bir hacmi gömen veya belirtilmiş bir yola gömülmüş hacmi içeren konteynerleri filtrele:
```shell
docker ps --filter="volume={{örnek/dizin}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"
```
{% endraw %}