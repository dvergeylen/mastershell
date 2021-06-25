---
layout: default
title: "rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rm">
  <a href="/id/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menghapus berkas atau direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/rm>.

#### Menghapus berkas dari lokasi manapun:
```shell
rm {{alamat/ke/berkas}} {{alamat/ke/berkas/lainnya}}
```
#### Menghapus direktori dan semua subdirektorinya secara rekursif:
```shell
rm -r {{alamat/ke/direktori}}
```
#### Menghapus direktori secara paksa, tanpa meminta konfirmasi atau menampilkan pesan kesalahan:
```shell
rm -rf {{alamat/ke/direktori}}
```
#### Menghapus banyak berkas secara interaktif, dengan meminta konfirmasi sebelum setiap penghapusan:
```shell
rm -i {{(beberapa)_berkas}}
```
#### Menghapus berkas dengan mode verbose, mencetak pesan untuk setiap berkas yang terhapus:
```shell
rm -v {{alamat/ke/directori/*}}
```
{% endraw %}