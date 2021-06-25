---
layout: default
title: "docker compose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-compose">
  <a href="/tr/common/docker-compose.html">docker compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çoklu konteynerli docker uygulamalarını çalıştırın ve yönetin.
> Daha fazla bilgi için: <https://docs.docker.com/compose/reference/overview/>.

#### Tüm konteynerleri listele:
```shell
docker-compose ps
```
#### Mevcut dizinde bir `docker-compose.yml` dosyası çalıştırarak arkaplandaki tüm konteynerleri çalıştırın ve başlatın:
```shell
docker-compose up -d
```
#### Tüm konteynerleri çalıştırın ve gerekiyorsa yeniden oluşturun:
```shell
docker-compose up --build
```
#### Tüm konteynerleri alternatif bir beste dosyasıyla başlatın:
```shell
docker-compose --file {{yoldan/dosyaya}} up
```
#### Çalışan tüm konteynerleri durdurun:
```shell
docker-compose stop
```
#### Tüm konteynerleri, ağları, imgeleri ve alanları durdurun ve silin:
```shell
docker-compose down --rmi all --volumes
```
#### Tüm konteynerler için logları takip edin:
```shell
docker-compose logs --follow
```
#### Belirtilmiş bir konteyner için logları takip edin:
```shell
docker-compose logs --follow {{konteyner_ismi}}
```
{% endraw %}