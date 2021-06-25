---
layout: default
title: "tldr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr">
  <a href="/tr/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komut satırı araçları için tldr-pages projesinden basit yardım sayfaları görüntüler.
> Daha fazla bilgi için: <https://tldr.sh>.

#### Bir komutun tipik kullanımını göster (ipucu: burayı görüntülemek için kullandığınız komutun aynısı!):
```shell
tldr {{komut}}
```
#### Linux için tar tldr sayfasını göster:
```shell
tldr -p {{linux}} {{tar}}
```
#### Bir Git alt komutu için yardım al:
```shell
tldr {{git-checkout}}
```
#### (Eğer alıcı önbellek oluşumunu destekliyorsa) Yerel paketleri güncelle:
```shell
tldr -u
```
{% endraw %}