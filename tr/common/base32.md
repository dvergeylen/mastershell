---
layout: default
title: "base32"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base32">
  <a href="/tr/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir dosya veya standart veriyi Base32 formatında şifrele veya yalın veri çıktısı olarak deşifre et.
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/base32>.

#### Bir dosyayı şifrele:
```shell
base32 {{dosyaismi}}
```
#### Bir dosyayı deşifre et:
```shell
base32 --decode {{dosyaismi}}
```
#### stdin'den şifrele:
```shell
{{herhangibirkomut}} | base32
```
#### stdin'den deşifre et:
```shell
{{herhangibirkomut}} | base32 --decode
```
{% endraw %}