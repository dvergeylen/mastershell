---
layout: default
title: "nvim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nvim">
  <a href="/id/common/nvim.html">nvim</a> <a href="#nvim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Neovim, teks editor programmer berbasis Vim, menyediakan beberapa mode untuk manipulasi teks berbeda jenis.
> Tekan `i` masuk mode edit. `<Esc>` kembali ke mode normal, yang tidak mengizinkan penyisipan teks biasa.
> Informasi lebih lanjut: <https://neovim.io>.

#### Membuka berkas:
```shell
nvim {{berkas}}
```
#### Masuk ke mode pengeditan teks (insert mode):
```shell
<Esc>i
```
#### Menyalin ("yank") atau memotong ("delete") baris saat ini (tempel itu dengan `P`):
```shell
<Esc>{{yy|dd}}
```
#### Batalkan operasi terakhir:
```shell
<Esc>u
```
#### Mencari sebuah pattern pada berkas (tekan `n`/`N` untuk pergi ke kecocokan berikutnya/sebelumnya):
```shell
<Esc>/{{pattern_pencarian}}<Enter>
```
#### Melakukan penggantian ekspresi reguler pada seluruh berkas:
```shell
<Esc>:%s/{{ekspresi_reguler}}/{{pengganti}}/g<Enter>
```
#### Menyimpan (write) berkas, dan keluar:
```shell
<Esc>:wq<Enter>
```
#### Keluar tanpa menyimpan:
```shell
<Esc>:q!<Enter>
```
{% endraw %}