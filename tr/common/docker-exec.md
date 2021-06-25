---
layout: default
title: "docker exec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-exec">
  <a href="/tr/common/docker-exec.html">docker exec</a> <a href="#docker-exec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Halihazırda çalışan bir Docker konteyneri üstünde komut çalıştır.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/komutline/exec/>.

#### Halihazırda çalışan bir konteynerin üstünde interaktif bir kabuk oturumunu çalıştır:
```shell
docker exec --interactive --tty {{konteyner_ismi}} {{/bin/bash}}
```
#### Halihazırda çalışan bir konteynerin üstüne arkaplanda çalışmak üzere (ayrılmış) bir komut çalıştır:
```shell
docker exec --detach {{konteyner_ismi}} {{komut}}
```
#### Belirtilen bir komutu üstünde çalıştırmak adına çalışan dizini seç:
```shell
docker exec --interactive -tty --workdir {{örnek/dizin}} {{konteyner_ismi}} {{komut}}
```
#### Varolan konteyner üstünde arkaplanda çalışmak üzere bir komut çalıştır ancak stdin'i açık tut:
```shell
docker exec --interactive --detach {{konteyner_ismi}} {{komut}}
```
#### Çalışmakta olan bir bash oturumu içinde bir çevre değişkeni belirle:
```shell
docker exec --interactive --tty --env {{değişken_ismi}}={{value}} {{konteyner_ismi}} {{/bin/bash}}
```
#### Belirtilmiş bir kullanıcı olarak komut çalıştır:
```shell
docker exec --user {{kullanıcı}} {{konteyner_ismi}} {{komut}}
```
{% endraw %}