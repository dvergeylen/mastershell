---
layout: default
title: "pacman --remove"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---remove">
  <a href="/tr/linux/pacman-remove.html">pacman --remove</a> <a href="#pacman---remove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Bu alt komut için yardım göster:
```shell
pacman --remove --help
```
#### Bir paket ve bağlılıklarını sil:
```shell
sudo pacman --remove --recursive {{paket_ismi}}
```
#### Bir paketi ve onun hem bağlılıklarını, hem de konfigürasyon dosyalarını sil:
```shell
sudo pacman --remove --recursive --nosave {{paket_ismi}}
```
#### Bir paketi telkin olmaksızın sil:
```shell
sudo pacman --remove --noconfirm {{paket_ismi}}
```
#### Yetim (başka bir pakete bağlılık olarak indirilmiş ancak herhangi bir paket tarafından gerektirilmeyen) paketleri sil:
```shell
sudo pacman --remove --recursive --nosave $(pacman --query --unrequired --deps --quiet)
```
#### Bir paketi ve ona bağlı olan tüm öbür paketleri sil:
```shell
sudo pacman --remove --cascade {{paket_ismi}}
```
#### (Bir paketin silinme durumunda) Etkilenecek paketleri (silmeden) listele:
```shell
pacman --remove --print {{paket_ismi}}
```
{% endraw %}