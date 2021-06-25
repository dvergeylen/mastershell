---
layout: default
title: "minetest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minetest">
  <a href="/tr/common/minetest.html">minetest</a> <a href="#minetest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çok oyunculu sınırsız dünyalı bloklu sandbox oyun motoru.
> Ayrıca `minetestserver` sayfasına bakılması önerilir.
> Daha fazla bilgi için: <https://wiki.minetest.net/Minetest>.

#### Minetest'i kullanıcı modunda başlat:
```shell
minetest
```
#### Minetest'i belirtilen dünyayı host edecek şekilde sunucu modunda başlat:
```shell
minetest --server --world {{isim}}
```
#### Belirtilmiş bir dosyaya geçmişi yaz:
```shell
minetest --logfile {{örnek/dosya}}
```
#### Hataları yalnızca konsola yaz:
```shell
minetest --quiet
```
{% endraw %}