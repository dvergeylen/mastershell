---
layout: default
title: "pacman --query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---query">
  <a href="/tr/linux/pacman-query.html">pacman --query</a> <a href="#pacman---query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Yüklenmiş paket ve sürümleri sırala:
```shell
pacman --query
```
#### Sadece özellikle indirilmiş paket ve sürümleri sırala:
```shell
pacman --query --explicit
```
#### Hangi paketin belirtilen dosyaya sahip olduğunu bul:
```shell
pacman --query --owns {{dosya_ismi}}
```
#### İndirilmiş bir pakete dair bilgiyi görüntüle:
```shell
pacman --query --info {{paket_ismi}}
```
#### Bir paketin içerdiği dosyaları sırala:
```shell
pacman --query --list {{paket_ismi}}
```
#### Yetim (başka bir pakete bağlılık olarak indirilmiş ancak herhangi bir paket tarafından gerektirilmeyen) paketleri sırala:
```shell
pacman --query --unrequired --deps --quiet
```
#### Mevcut depolarda bulunmayan, indirilmiş paketleri sırala:
```shell
pacman --query --foreign
```
#### Miadı dolmuş paketleri sırala:
```shell
pacman --query --upgrades
```
{% endraw %}