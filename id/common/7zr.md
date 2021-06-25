---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/id/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengarsip file dengan rasio kompresi yang tinggi.
> Serupa dengan `7z` namun mendukung format file arsip `.7z` saja.
> Informasi lebih lanjut: <https://www.7-zip.org>.

#### Meng[a]rsipkan sebuah file atau direktori:
```shell
7zr a {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Mengenkripsi sebuah file arsip (termasuk nama-nama file yang terkandung di dalamnya):
```shell
7zr a {{jalan/menuju/arsip_terenkripsi.7z}} -p{{kata sandi}} -mhe=on {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip dengan mempertahankan struktur direktori asli:
```shell
7zr x {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip ke dalam direktori yang ditentukan:
```shell
7zr x {{jalan/menuju/arsip.7z}} -o{{jalan/menuju/direktori}}
```
#### Mengekstrak sebuah file arsip menuju stdout:
```shell
7zr x {{jalan/menuju/arsip.7z}} -so
```
#### Me[l]ihat daftar isi dari sebuah file arsip:
```shell
7zr l {{path/to/archive.7z}}
```
#### Mengetahui daftar format file arsip yang didukung:
```shell
7zr i
```
{% endraw %}