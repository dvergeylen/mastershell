---
layout: default
title: "pacman --sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---sync">
  <a href="/tr/linux/pacman-sync.html">pacman --sync</a> <a href="#pacman---sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Yeni bir paket indir::
```shell
sudo pacman --sync {{paket_ismi}}
```
#### Tüm paketleri senkronize et ve güncelle (bahsi geçen paketleri güncellemeden indirmek için `--downloadonly` eki gereklidir)
```shell
sudo pacman --sync --refresh --sysupgrade
```
#### Tüm paketleri güncelle ve telkin olmaksızın yeni bir tane indir:
```shell
sudo pacman --sync --refresh --sysupgrade --noconfirm {{paket_ismi}}
```
#### Paket veritabanını girilen ifade ile arat:
```shell
pacman --sync --search "{{arama_şablonu}}"
```
#### Bir paket hakkında bilgi görüntüle:
```shell
pacman --sync --info {{paket_ismi}}
```
#### Bir paket güncellemesi sırasında çakışan dosyaların üstüne yaz:
```shell
sudo pacman --sync --refresh --sysupgrade --overwrite {{örnek_dosya}}
```
#### Tüm paketleri senkronize et ve güncelle, ancak belli bir paketi yoksay:
```shell
sudo pacman --sync --refresh --sysupgrade --ignore {{paket_ismi}}
```
#### Kullanılmayan paket ve kullanılmamış depoları çerezlerden sil (tüm paketlerin çerezlerini temizlemek için `--clean` eki iki kez kullanılmalıdır):
```shell
sudo pacman --sync --clean
```
{% endraw %}