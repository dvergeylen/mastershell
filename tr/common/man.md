---
layout: default
title: "man"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="man">
  <a href="/tr/common/man.html">man</a> <a href="#man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kılavuz sayfalarını biçimlendir ve göster.
> Daha fazla bilgi için: <https://www.man7.org/linux/man-pages/man1/man.1.html>.

#### Bir komut için man sayfasını görüntüle:
```shell
man {{komut}}
```
#### Sayfanın 7. bölümündeki bir komut için man sayfasını görüntüle:
```shell
man {{komut}}.{{7}}
```
#### Mansayfaları için aratılan yolu göster:
```shell
man --path
```
#### Mansayfasını göstermek yerine mansayfasının konumunu göster:
```shell
man -w {{komut}}
```
#### Belirtilen ifadeyi içeren mansayfalarını ara:
```shell
man -k "{{aranan_ifade}}"
```
{% endraw %}