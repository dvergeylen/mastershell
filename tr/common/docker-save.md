---
layout: default
title: "docker save"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-save">
  <a href="/tr/common/docker-save.html">docker save</a> <a href="#docker-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla docker imgesini arşivlemek için dışa aktar.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/save/>.

#### Bir imgeyi, stdout'u tar arşivine yönlendirerek kaydet:
```shell
docker save {{imge}}:{{etiket}} > {örnek/dosya.tar}}
```
#### Bir imgeyi, bir tar arşivine kaydet:
```shell
docker save --output {{örnek/dosya.tar}} {{imge}}:{{etiket}}
```
#### Bir imgenin tüm etiketlerini kaydet:
```shell
docker save --output {{örnek/dosya.tar}} {{imge_ismi}}
```
#### Bir imgenin belirli etiketlerini kaydetmek için elle seç:
```shell
docker save --output {{örnek/dosya.tar}} {{imge_ismi:etiket1 imge_ismi:etiket2 ...}}
```
{% endraw %}