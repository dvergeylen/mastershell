---
layout: default
title: "pacman-mirrors"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman-mirrors">
  <a href="/tr/linux/pacman-mirrors.html">pacman-mirrors</a> <a href="#pacman-mirrors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manjaro Linux için pacman aynalistesi oluşturucu.
> pacman-mirrors'ın çalıştırıldığı her vakit, E`sudo pacman -Syyu` komutu ile veritabanının senkronize edilmesi ve sistemin güncellenmesi gerekir.
> Daha fazla bilgi için: <https://wiki.manjaro.org/index.php?title=Pacman-mirrors>.

#### Varsayılan ayarlar ile bir aynalistesi oluştur:
```shell
sudo pacman-mirrors --fasttrack
```
#### Mevcut aynaların durumunu göster:
```shell
pacman-mirrors --status
```
#### Mevcut dalı göster:
```shell
pacman-mirrors --get-branch
```
#### Farklı bir dala geç:
```shell
sudo pacman-mirrors --api --set-branch {{stabil|instabil|test_ediliyor}}
```
#### Sadece IP adresinin bulunduğu ülkenin aynalarını kullanarak bir aynalistesi oluştur:
```shell
sudo pacman-mirrors --geoip
```
{% endraw %}