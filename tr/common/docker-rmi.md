---
layout: default
title: "docker rmi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-rmi">
  <a href="/tr/common/docker-rmi.html">docker rmi</a> <a href="#docker-rmi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla Docker imgesini sil.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/rmi/>.

#### Yardım göster:
```shell
docker rmi
```
#### Bir veya daha fazla imgeyi isimlerini belirterek sil:
```shell
docker rmi {{imge1 imge2 ...}}
```
#### Bir imgeyi zorla sil:
```shell
docker rmi --force {{imge}}
```
#### Bir imgeyi etiketlenmemiş ana yollarını silmeden sil:
```shell
docker rmi --no-prune {{imge}}
```
{% endraw %}