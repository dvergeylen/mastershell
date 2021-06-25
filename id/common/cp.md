---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/id/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Membuat salinan file dan direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/cp>.

#### Membuat salinan file ke lokasi lain:
```shell
cp {{jalan/menuju/file_sumber.ext}} {{jalan/menuju/file_tujuan.ext}}
```
#### Menyalin file ke direktori lain, dengan nama yang sama:
```shell
cp {{jalan/menuju/file_sumber.ext}} {{jalan/menuju/direktori_tujuan}}
```
#### Menyalin sebuah direktori secara beserta isinya ke lokasi lain (jika tujuan sudah ada, direktori tersebut disalin ke dalamnya):
```shell
cp -R {{jalan/menuju/direktori_sumber}} {{jalan/menuju/direktori_tujuan}}
```
#### Menyalin sebuah direktori secara beserta isinya, dalam mode `verbose` (menampilkan file-file ketika disalin):
```shell
cp -vR {{jalan/menuju/direktori_sumber}} {{jalan/menuju/direktori_tujuan}}
```
#### Menyalin file-file teks ke lokasi lain, dalam mode interaktif (menampilkan pertanyaan sebelum menimpa):
```shell
cp -i {{*.txt}} {{jalan/menuju/direktori_tujuan}}
```
#### Melepaskan tautan simbolis sebelum menyalin:
```shell
cp -L {{tautan}} {{jalan/menuju/direktori_tujuan}}
```
{% endraw %}