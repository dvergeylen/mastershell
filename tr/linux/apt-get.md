---
layout: default
title: "apt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-get">
  <a href="/tr/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian ve Ubuntu paket yönetim aracı.
> Paket aramak için `apt-cache` komutunu kullanın.
> Daha fazla bilgi için: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Kullanılabilir paket ve versiyon listesini güncelleyin (diğer `apt-get` komutlarını çalıştırmadan önce kullanmanız önerilir):
```shell
apt-get update
```
#### Bir paket yükleyin veya son sürüme güncelleyin:
```shell
apt-get install {{paket}}
```
#### Bir paketi silin:
```shell
apt-get remove {{paket}}
```
#### Bir paketi ve konfigürasyon dosyalarını silin:
```shell
apt-get purge {{paket}}
```
#### Yüklü paketlerin hepsini son sürümlerine yükseltin:
```shell
apt-get upgrade
```
#### Yerel depoyu temizleyin - kullanılmayan gereksiz paket dosyalarını (.deb) silin:
```shell
apt-get autoclean
```
#### Artık gerekmeyen paketleri silin:
```shell
apt-get autoremove
```
#### Yüklenmiş paketleri yükseltin (`upgrade` gibi), ancak gereksiz paketleri silin ve yeni bağımlılıkları memnun edecek ek paketler kurun:
```shell
apt-get dist-upgrade
```
{% endraw %}