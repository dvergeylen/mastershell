---
layout: default
title: "minetestserver"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minetestserver">
  <a href="/tr/common/minetestserver.html">minetestserver</a> <a href="#minetestserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çok oyunculu sınırsız dünyalı bloklu sanbox sunucusu.
> Ayrıca `minetest` sayfasına bakılması önerilir.
> Daha fazla bilgi için: <https://wiki.minetest.net/Setting_up_a_server>.

#### Sunucuyu başlar:
```shell
minetestserver
```
#### Müsait dünyaları sırala:
```shell
minetestserver --world list
```
#### Yüklenecek dünya ismini belirt:
```shell
minetestserver --world {{dunya_ismi}}
```
#### Müsait oyun ID'lerini sırala:
```shell
minetestserver --gameid list
```
#### Kullanılacak oyunu belirt:
```shell
minetestserver --gameid {{oyun_id'si}}
```
#### Belirtilmiş bir port'u dinle:
```shell
minetestserver --port {{34567}}
```
#### Başka bir veritabanı yazılımına göç et:
```shell
minetestserver --migrate {{sqlite3|leveldb|redis}}
```
#### Sunucuyu başlattıktan sonra interaktif bir terminal aç:
```shell
minetestserver --terminal
```
{% endraw %}