---
layout: default
title: "pacman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman">
  <a href="/tr/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Tüm paketleri senkronize et ve güncelle:
```shell
pacman -Syu
```
#### Yeni bir paket indir:
```shell
pacman -S {{paket_ismi}}
```
#### Bir paket ve bağlılıklarını sil:
```shell
pacman -Rs {{paket_ismi}}
```
#### Paket veritabanını girilen ifade ile arat:
```shell
pacman -Ss "{{arama_şablonu}}"
```
#### İndirilmiş paket ve sürümleri sırala:
```shell
pacman -Q
```
#### Sadece özellikle belirtilen paket ve sürümleri sırala:
```shell
pacman -Qe
```
#### Hangi paketin belirtilen dosyaya sahip olduğunu bul:
```shell
pacman -Qo {{dosya_ismi}}
```
#### Paket çerezlerini boş alan açmak için temizle:
```shell
pacman -Scc
```
{% endraw %}