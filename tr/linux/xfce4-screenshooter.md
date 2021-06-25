---
layout: default
title: "xfce4-screenshooter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xfce4-screenshooter">
  <a href="/tr/linux/xfce4-screenshooter.html">xfce4-screenshooter</a> <a href="#xfce4-screenshooter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> XFCE4 ekran görüntüsü aracı.
> Daha fazla bilgi için: <https://docs.xfce.org/apps/xfce4-screenshooter/start>.

#### Ekran görüntüsü alma grafik arayüzünü başlat:
```shell
xfce4-screenshooter
```
#### Tüm ekranın ekran görüntüsünü al ve nasıl devam edileceğini belirlemek adına grafik arayüzünü başlat:
```shell
xfce4-screenshooter --fullscreen
```
#### Tüm ekranın ekran görüntüsünü al ve görüntüyü belirtilen dizine kaydet:
```shell
xfce4-screenshooter --fullscreen --save {{örnek/dizin}}
```
#### Ekran görüntüsünü çekmeden önce belli bir süre bekle:
```shell
xfce4-screenshooter --delay {{saniye_miktarı}}
```
#### Ekranın (fare ile seçilecek) belli bir bölümünün görüntüsünü al:
```shell
xfce4-screenshooter --region
```
#### Üzerinde bulunulan pencerenin görüntüsünü al ve panoya kopyala:
```shell
xfce4-screenshooter --window --clipboard
```
#### Üzerinde bulunulan pencerenin görüntüsünü qal ve seçilen bir program ile aç:
```shell
xfce4-screenshooter --window --open {{gimp}}
```
{% endraw %}