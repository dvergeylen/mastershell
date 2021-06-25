---
layout: default
title: "aptitude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aptitude">
  <a href="/tr/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian ve Ubuntu paket yönetim aracı.
> Daha fazla bilgi için: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Kullanılabilir paket ve sürüm listesini senkronize et. Bu, herhangi bir aptitude komutunu uygulamadan önce çalıştırılmalıdır:
```shell
aptitude update
```
#### Yeni bir paket ve onun bağımlılıklarını kur:
```shell
aptitude install {{paket}}
```
#### Paket ara:
```shell
aptitude search {{paket}}
```
#### İndirilmiş bir paket ara: (`?installed` bir aptitude arama ifadesidir):
```shell
aptitude search '?installed({{paket}})'
```
#### Bir paket ve onun bağımlılıklarını kaldır:
```shell
aptitude remove {{paket}}
```
#### Yüklü paketleri son kullanılabilir sürümlerine yükselt:
```shell
aptitude upgrade
```
#### Yüklü paketleri yükle (`aptitude upgrade` gibi), gereksizleri sil ve yeni bağımlılıkları karşılamak üzere ek paketler kur:
```shell
aptitude full-upgrade
```
#### Bir paketin otomatik yükseltilmesini engellemek için onu beklemede tut:
```shell
aptitude hold '?installed({{paket}})'
```
{% endraw %}