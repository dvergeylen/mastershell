---
layout: default
title: "docker images"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-images">
  <a href="/tr/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker imgelerini yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/images/>.

#### Tüm Docker imgelerini listele:
```shell
docker images
```
#### Orta düzeyler de dahil olmak üzere tüm Docker imgelerini sırala:
```shell
docker images --all
```
#### Çıktıyı sessiz modda (yalnızca sayısal ID'ler olarak) sırala:
```shell
docker images --quiet
```
#### Herhangi bir konteyner tarafından kullanılmayan tüm Docker imgelerini sırala:
```shell
docker images --filter dangling=true
```
#### İsminde belirtilen dizeleri taşıyan imgeleri sırala:
```shell
docker images "{{*isim*}}"
```
{% endraw %}