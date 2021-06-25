---
layout: default
title: "adb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb">
  <a href="/id/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: berkomunikasi dengan emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Cek apakah proses server adb telah dimulai dan memulainya:
```shell
adb start-server
```
#### Menghentikan proses server adb:
```shell
adb kill-server
```
#### Memulai shell jarak jauh pada emulator/perangkat tujuan:
```shell
adb shell
```
#### Menginstal aplikasi Android ke emulator/perangkat tujuan:
```shell
adb install -r {{alamat/ke/berkas.apk}}
```
#### Menyalin berkas/direktori dari perangkat tujuan:
```shell
adb pull {{alamat/ke/berkas_atau_direktori_perangkat}} {{alamat/ke/direktori_lokal_tujuan}}
```
#### Menyalin berkas/direktori ke perangkat tujuan:
```shell
adb push {{alamat/ke/berkas_atau_direktori_lokal}} {{alamat/ke/direktori_perangkat_tujuan}}
```
#### Mendapatkan daftar perangkat yang terhubung:
```shell
adb devices
```
{% endraw %}