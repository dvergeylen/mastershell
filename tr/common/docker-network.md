---
layout: default
title: "docker network"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-network">
  <a href="/tr/common/docker-network.html">docker network</a> <a href="#docker-network"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker ağları oluştur ve yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/network/>.

#### docker daemon'daki tüm müsait ve düzenlenmiş ağları sırala:
```shell
docker network ls
```
#### Kullanıcı tarafından belirtilmiş bir ağ oluştur:
```shell
docker network create --driver {{driver_name}} {{ağ_ismi}}
```
#### Boşluk ile ayrılmış bir ağ listesinin detaylı bilgisini görüntüle:
```shell
docker network inspect {{ağ_ismi}}
```
#### Bir konteyneri isim veya ID kullanarak bir ağa bağla:
```shell
docker network connect {{ağ_ismi}} {{konteyner_ismi|ID}}
```
#### Bir konteyneri bir ağdan çıkar:
```shell
docker network disconnect {{ağ_ismi}} {{konteyner_ismi|ID}}
```
#### Tüm kullanılmayan (hiçbir konteyner tarafından belirtilmeyen) ağları sil:
```shell
docker network prune
```
#### Kullanılmayan ağların boşluk ile ayrılmış bir listesini sil:
```shell
docker network rm {{ağ_ismi}}
```
{% endraw %}