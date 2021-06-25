---
layout: default
title: "chroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chroot">
  <a href="/tr/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komut veya etkileşimli komut satırını özel kök diziniyle çalıştırır.
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/chroot>.

#### Komutu yeni kök dizini olarak çalıştır:
```shell
chroot {{yeni/kok/yolu}} {{komut}}
```
#### Kullanılacak kullanıcı ve grubu (ID veya isim) belirle:
```shell
chroot --userspec={{kullanici:grup}}
```
{% endraw %}