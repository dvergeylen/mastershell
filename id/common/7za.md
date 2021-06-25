---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/id/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengarsip file dengan rasio kompresi yang tinggi.
> Serupa dengan `7z` namun mendukung lebih sedikit format file arsip dan dapat digunakan lintas sistem operasi.
> Informasi lebih lanjut: <https://www.7-zip.org>.

#### Meng[a]rsipkan sebuah file atau direktori:
```shell
7za a {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Mengenkripsi sebuah file arsip (termasuk nama-nama file yang terkandung di dalamnya):
```shell
7za a {{jalan/menuju/arsip_terenkripsi.7z}} -p{{kata sandi}} -mhe=on {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip dengan mempertahankan struktur direktori asli:
```shell
7za x {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip ke dalam direktori yang ditentukan:
```shell
7za x {{jalan/menuju/arsip.7z}} -o{{jalan/menuju/direktori}}
```
#### Mengekstrak sebuah file arsip menuju stdout:
```shell
7za x {{jalan/menuju/arsip.7z}} -so
```
#### Meng[a]rsipkan file atau direktori menggunakan format file arsip tertentu:
```shell
7za a -t{{7z|zip|gzip|bzip2|lzip}} {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Me[l]ihat daftar isi dari sebuah file arsip:
```shell
7za l {{path/to/archive.7z}}
```
#### Mengetahui daftar format file arsip yang didukung:
```shell
7za i
```
{% endraw %}