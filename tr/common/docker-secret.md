---
layout: default
title: "docker secret"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-secret">
  <a href="/tr/common/docker-secret.html">docker secret</a> <a href="#docker-secret"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker swarm sırlarını yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/secret/>.

#### stdin'den yeni bir sır yarat:
```shell
{{komut}} | docker secret create {{sır_ismi}} -
```
#### Bir dosyadan yeni sır oluşturun:
```shell
docker secret create {{sır_ismi}} {{örnek/dosya}}
```
#### Tüm sırları sırala:
```shell
docker secret ls
```
#### Bir veya daha fazla sırra dair detaylı bilgiyi insan dostu bir formatta göster:
```shell
docker secret inspect --pretty {{sır_ismi1 sır_ismi2 ...}}
```
#### Bir veya daha fazla sırrı sil:
```shell
docker secret rm {{sır_ismi1 sır_ismi2 ...}}
```
{% endraw %}