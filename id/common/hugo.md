---
layout: default
title: "hugo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hugo">
  <a href="/id/common/hugo.html">hugo</a> <a href="#hugo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Penghasil website statis berbasis template. Menggunakan modul, komponen dan tema.
> Informasi lebih lanjut: <https://gohugo.io>.

#### Membuat website Hugo baru:
```shell
hugo new site {{alamat/ke/website}}
```
#### Membuat tema Hugo baru (tema juga dapat diunduh dari https://themes.gohugo.io/):
```shell
hugo new theme {{nama_tema}}
```
#### Membuat halaman baru:
```shell
hugo new {{nama_bagian}}/{{nama_berkas}}
```
#### Menbuild website ke direktori `./public`:
```shell
hugo
```
#### Menbuild website termasuk halaman yang ditandai sebagai "draft":
```shell
hugo --buildDrafts
```
#### Menbuild website ke direktori yang ditentukan:
```shell
hugo --destination {{alamat/tujuan}}
```
#### Menbuild website, memulai webserver untuk menyajikannya, dan secara otomatis memuat ulang jika ada halaman yang berubah:
```shell
hugo server
```
{% endraw %}