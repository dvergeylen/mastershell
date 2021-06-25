---
layout: default
title: "touch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="touch">
  <a href="/id/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengubah waktu akses (atime) dan waktu modifikasi (mtime) dari sebuah file.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/touch>.

#### Membuat file baru yang kosong atau mengubah waktu file yang telahj ada ke waktu sekarang:
```shell
touch {{nama_file}}
```
#### Mengatur waktu sebuah file ke tanggal dan jam tertentu:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{nama_file}}
```
#### Menggunakan waktu dari satu file untuk mengatur waktu file yang lain:
```shell
touch -r {{nama_file}} {{nama_file2}}
```
{% endraw %}