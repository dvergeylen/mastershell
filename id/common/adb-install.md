---
layout: default
title: "adb install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-install">
  <a href="/id/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: Menginstal paket ke emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Menginstal aplikasi Android ke emulator/perangkat:
```shell
adb install {{alamat/ke/berkas.apk}}
```
#### Menginstal ulang aplikasi yang sudah ada, menjaga datanya:
```shell
adb install -r {{alamat/ke/berkas.apk}}
```
#### Memberikan semua izin yang terdaftar di manifest aplikasi:
```shell
adb install -g {{alamat/ke/berkas.apk}}
```
#### Memperbarui langsung paket terinstal dengan hanya memperbarui bagian dari APK yang berubah:
```shell
Adb install --fastdeploy {{alamat/ke/berkas.apk}}
```
{% endraw %}