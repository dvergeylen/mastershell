---
layout: default
title: "docker run"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-run">
  <a href="/tr/common/docker-run.html">docker run</a> <a href="#docker-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yeni bir Docker konteynerinde bir komut çalıştır.
> Daha fazla bilgi: <https://docs.docker.com/engine/reference/commandline/run/>.

#### Yeni bir konteynerde, etiketlenmiş bir imgeden komut çalıştır.:
```shell
docker run {{imge:etiket}} {{komut}}
```
#### Yeni bir konteynerde arkaplanda çalışacak şekilde komut çalıştır ve ID'sini göster:
```shell
docker run -d {{imge}} {{komut}}
```
#### İnteraktif mod ve pseudo-TTY'deki bir açık-kapalı konteynerde komut çalıştır:
```shell
docker run --rm -it {{imge}} {{komut}}
```
#### Yeni bir konteynerde geçebilmiş çevresel değişkenler ile komut çalıştır:
```shell
docker run -e '{{değişken}}={{değer}}' -e {{değişken}} {{imge}} {{komut}}
```
#### Yeni bir konteynerde bağlama takılı hacimlerle komut çalıştır:
```shell
docker run -v {{örnek/host}}:{{örnek/konteyner}} {{imge}} {{komut}}
```
#### Yayınlanmış portları içeren yeni bir konteynerde komut çalıştır:
```shell
docker run -p {{host_portu}}:{{konteyner_portu}} {{imge}} {{komut}}
```
{% endraw %}