---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#cd">cd</a>
* <a href="#chkdsk">chkdsk</a>
* <a href="#cls">cls</a>
* <a href="#dir">dir</a>
* <a href="#find">find</a>
* <a href="#ipconfig">ipconfig</a>
* <a href="#ver">ver</a>

{% raw %}
<h2 id="cd">
  <a href="/id/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan nama atau ganti direktori saat ini.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Menuju suatu direktori pada drive yang sama:
```shell
cd {{lokasi/ke/direktori}}
```
#### Menampilkan nama dari direktori saat ini:
```shell
cd
```
#### Menuju ke induk direktori dari direktori saat ini:
```shell
cd ..
```
#### Menuju direktori di dalam suatu drive:
```shell
cd {{lokasi/ke/direktori}} /d
```
{% endraw %}{% raw %}
<h2 id="chkdsk">
  <a href="/id/windows/chkdsk.html">chkdsk</a> <a href="#chkdsk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Memeriksa dan mencari kesalahan dalam sebuah sistem file dan metadata volume penyimpanan.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/chkdsk>.

#### Memeriksa sebuah ruang penyimpanan berdasarkan huruf drive (diakhiri dengan titik dua), lokasi pemasangan, atau nama ruang:
```shell
chkdsk {{ruang_penyimpanan}}
```
#### Memperbaiki kesalahan pada ruang penyimpanan yang ditentukan:
```shell
chkdsk {{ruang_penyimpanan}} /f
```
#### Melepas ruang penyimpanan tertentu untuk pemeriksaan:
```shell
chkdsk {{ruang_penyimpanan}} /x
```
#### Mengubah ukuran file log dalam sebuah ruang penyimpanan dengan sistem file NTFS:
```shell
chkdsk /l{{ukuran}}
```
{% endraw %}{% raw %}
<h2 id="cls">
  <a href="/id/windows/cls.html">cls</a> <a href="#cls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Membersihkan layar.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/cls>.

#### Bersihkan layar:
```shell
cls
```
{% endraw %}{% raw %}
<h2 id="dir">
  <a href="/id/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lis isi direktori.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### Tampilkan isi direktori saat ini:
```shell
dir
```
#### Tampilkan isi direktori yang ditentukan:
```shell
dir {{lokasi/ke/direktori}}
```
#### Tampilkan isi dari direktori saat ini, termasuk yang disembunyikan:
```shell
dir /A
```
#### Tampilkan isi direktori yang ditentukan, termasuk yang disembunyikan:
```shell
dir {{lokasi/ke/direktori}} /A
```
{% endraw %}{% raw %}
<h2 id="find">
  <a href="/id/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mencari teks tertentu di dalam suatu file atau direktori.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### Mencari baris-baris dalam file yang mengandung teks tertentu:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}}
```
#### Menunjukkan baris-baris dalam file yang tidak mengandung teks tertentu:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}} /v
```
#### Menghitung jumlah baris dalam file yang mengandung teks tertentu:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}} /c
```
#### Mencari baris-baris dalam file yang mengandung teks tertentu beserta nomor barisnya:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}} /n
```
{% endraw %}{% raw %}
<h2 id="ipconfig">
  <a href="/id/windows/ipconfig.html">ipconfig</a> <a href="#ipconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan dan mengatur konfigurasi jaringan dalam sistem operasi Windows.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/ipconfig>.

#### Menunjukkan daftar adaptor jaringan:
```shell
ipconfig
```
#### Menunjukkan daftar adaptor jaringan secara lengkap:
```shell
ipconfig /all
```
#### Memperbarui alamat IP sebuah adaptor jaringan:
```shell
ipconfig /renew {{adaptor}}
```
#### Mengosongkan alamat-alamat IP yang disetel dalam sebuah adaptor jaringan:
```shell
ipconfig /release {{adaptor}}
```
#### Mengosongkan cache DNS:
```shell
ipconfig /flushdns
```
{% endraw %}{% raw %}
<h2 id="ver">
  <a href="/id/windows/ver.html">ver</a> <a href="#ver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan nomor versi Windows atau MS-DOS saat ini.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/ver>.

#### Menampilkan nomor versi saat ini:
```shell
ver
```
{% endraw %}