---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/tr/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir dosya veya standart veriyi Base64 formatında şifrele veya yalın veri çıktısı olarak deşifre et.
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/base64>.

#### Bir dosyayı şifrele:
```shell
base64 {{dosyaismi}}
```
#### Bir dosyayı deşifre et:
```shell
base64 --decode {{dosyaismi}}
```
#### stdin'den şifrele:
```shell
{{herhangibirkomut}} | base64
```
#### stdin'den deşifre et:
```shell
{{herhangibirkomut}} | base64 --decode
```
{% endraw %}