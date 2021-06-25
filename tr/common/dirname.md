---
layout: default
title: "dirname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirname">
  <a href="/tr/common/dirname.html">dirname</a> <a href="#dirname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Belirtilen dosya veya yolun ana dizinini hesaplar.
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/dirname>.

#### Belirtilen yolun ana dizinini hesapla:
```shell
dirname {{dosya_veya_dizine/giden/yol}}
```
#### Birden çok yolun ana dizinini hesapla:
```shell
dirname {{dosya_veya_dizine/giden/yol_1}} {{dosya_veya_dizine/giden/yol_2}}
```
#### Komut çıktısını yeni satır yerine NUL karakteri ile sınırlandırma (`xargs` yazılımı ile kullanırken işe yarar):
```shell
dirname --zero {{dosya_veya_dizine/giden/yol_1}} {{dosya_veya_dizine/giden/yol_2}}
```
{% endraw %}