---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/id/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan daftar konten pada direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/ls>.

#### Menampilkan daftar berkas dengan satu item tiap baris:
```shell
ls -1
```
#### Menampilkan daftar semua berkas, termasuk berkas tersembunyi:
```shell
ls -a
```
#### Menampilkan daftar semua berkas, dengan akhiran `/` ditambahkan ke nama direktori:
```shell
ls -F
```
#### Menampilkan daftar berformat panjang (menampilkan izin, kepemilikan, ukuran dan waktu modifikasi pada setiap berkas):
```shell
ls -la
```
#### Menampilkan daftar berformat panjang dan ukuran ditampilkan menggunakan unit yang mudah dibaca manusia (KiB, MiB, GiB):
```shell
ls -lh
```
#### Menampilkan daftar berformat panjang dan diurutkan berdasarkan ukuran (menurun):
```shell
ls -lS
```
#### Menampilkan daftar berformat panjang dari semua berkas dan diurutkan berdasarkan tanggal modifikasi (terlama dulu):
```shell
ls -ltr
```
{% endraw %}