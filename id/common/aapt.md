---
layout: default
title: "aapt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aapt">
  <a href="/id/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alat Pemaketan Android Asset.
> Menyusun dan memaketkan resource aplikasi Android.

#### Daftar berkas-berkas yang termuat dalam arsip APK:
```shell
aapt list {{alamat/ke/aplikasi.apk}}
```
#### Menampilkan metadata aplikasi (versi, izin, dsb.):
```shell
aapt dump badging {{alamat/ke/aplikasi.apk}}
```
#### Membuat arsip APK baru dengan berkas dari direktory yang ditentukan:
```shell
aapt package -F {{alamat/ke/aplikasi.apk}} {{alamat/ke/direktori}}
```
{% endraw %}