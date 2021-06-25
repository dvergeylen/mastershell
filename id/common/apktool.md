---
layout: default
title: "apktool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apktool">
  <a href="/id/common/apktool.html">apktool</a> <a href="#apktool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Me-reverse engineer berkas APK.
> Informasi lebih lanjut: <https://ibotpeaches.github.io/Apktool/>.

#### Dekode berkas APK:
```shell
apktool d {{berkas.apk}}
```
#### Men-build folder menjadi berkas APK:
```shell
apktool b {{alamat/ke/direktori}}
```
#### Menginstal dan menyimpan frameworks:
```shell
apktool if {{framework.apk}}
```
{% endraw %}