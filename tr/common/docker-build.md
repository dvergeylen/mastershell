---
layout: default
title: "docker build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-build">
  <a href="/tr/common/docker-build.html">docker build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir Dockerfile'dan imge yaratın.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/build/>.

#### Mevcut dizindeki Dockerfile'dan bir docker imgesi oluşturun:
```shell
docker build .
```
#### Belirtilen URL'deki Dockerfile'dan bir docker imgesi oluşturun:
```shell
docker build {{ornekadres.com/ornek-dizin/ornek-docker-projesi}}
```
#### Bir docker imgesi oluşturun ve etiketleyin:
```shell
docker build --tag {{isim:etiket}} .
```
#### İmge oluştururken çerez kullanımını etkisizleştirin:
```shell
docker build --no-cache --tag {{isim:etiket}} .
```
#### Belirtilen Dockerfile ile bir docker imgesi oluşturun:
```shell
docker build --file {{Dockerfile}} .
```
#### Kişiselleştirilmiş yapım-zaman değerleriyle oluşturun:
```shell
docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .
```
{% endraw %}