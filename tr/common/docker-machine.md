---
layout: default
title: "docker-machine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-machine">
  <a href="/tr/common/docker-machine.html">docker-machine</a> <a href="#docker-machine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker çalıştıran makineler oluştur ve onları yönet.
> Daha fazla bilgi için: <https://docs.docker.com/machine/reference/>.

#### Halihazırda çalışan docker makinelerini sırala:
```shell
docker-machine ls
```
#### Belirli bir isim ile docker makinesi oluştur:
```shell
docker-machine create {{isim}}
```
#### Bir makinenin durumunu öğren:
```shell
docker-machine status {{isim}}
```
#### Bir makineyi başlat:
```shell
docker-machine start {{isim}}
```
#### Bir makineyi durdur:
```shell
docker-machine stop {{isim}}
```
#### Bir makine hakkındaki bilgileri incele:
```shell
docker-machine inspect {{isim}}
```
{% endraw %}