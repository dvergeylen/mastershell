---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/id/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mencetak dan menggabungkan berkas.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/cat>.

#### Mencetak konten berkas ke keluaran standar:
```shell
cat {{berkas}}
```
#### Menggabungkan konten beberapa berkas ke berkas tujuan:
```shell
cat {{berkas1}} {{berkasw}} > {{berkas_tujuan}}
```
#### Menambahkan konten beberapa berkas ke berkas tujuan:
```shell
cat {{berkas1}} {{berkas2}} >> {{berkas_tujuan}}
```
#### Memberi nomor pada semua baris keluaran:
```shell
cat -n {{berkas}}
```
#### Menampilkan karakter yang tidak dapat dicetak dan spasi (dengan awalan `M-`jika non-ASCII):
```shell
cat -v -t -e {{berkas}}
```
{% endraw %}