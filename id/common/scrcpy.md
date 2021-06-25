---
layout: default
title: "scrcpy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scrcpy">
  <a href="/id/common/scrcpy.html">scrcpy</a> <a href="#scrcpy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tampilkan layar and kontrol perangkat Android anda di dalam desktop.
> Informasi lebih lanjut: <https://github.com/Genymobile/scrcpy>.

#### Tampilkan layar sebuah perangkat yang terhubung:
```shell
scrcpy
```
#### Tampilkan layar perangkat tertentu berdasarkan ID atau alamat IP-nya (temukan menggunakan perintah `adb devices`):
```shell
scrcpy --serial {{0123456789abcdef|192.168.0.1:5555}}
```
#### Tampilkan layar dalam mode layar penuh / fullscreen:
```shell
scrcpy --fullscreen
```
#### Putarkan tampilan layar perangkat dalam kelipatan 90 derajat (berlawanan arah jarum jam):
```shell
scrcpy --rotation {{0|1|2|3}}
```
#### Tunjukkan indikator sentuhan pada perangkat fisik:
```shell
scrcpy --show-touches
```
#### Rekam tampilan layar perangkat ke dalam file video tertentu:
```shell
scrcpy --record {{jalan/menuju/file.mp4}}
```
#### Tentukan direktori yang akan digunakan untuk memindahkan file (non-APK) ke dalam perangkat melalui drag-and-drop:
```shell
scrcpy --push-target {{jalan/menuju/direktori}}
```
{% endraw %}