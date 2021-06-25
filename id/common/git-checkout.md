---
layout: default
title: "git checkout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-checkout">
  <a href="/id/common/git-checkout.html">git checkout</a> <a href="#git-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checkout cabang atau alamat ke direktori kerja.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-checkout>.

#### Membuat dan beralih ke cabang baru:
```shell
git checkout -b {{nama_cabang}}
```
#### Membuat dan beralih ke cabang baru berdasarkan referensi tertentu (misal cabang, remote, cabang remote, dan tag):
```shell
git checkout -b {{nama_cabang}} {{referense}}
```
#### Beralih ke cabang lokal yang ada:
```shell
git checkout {{nama_cabang}}
```
#### Beralih ke cabang yang sebelumnya di checkout:
```shell
git checkout -
```
#### Beralih ke cabang remote yang ada:
```shell
git checkout --track {{nama_remote}}/{{nama_cabang}}
```
#### Menyingkirkan semua perubahan yang tidak masuk status stage pada direktori saat ini (lihat `git reset` untuk perintah yang lebih mirip undo):
```shell
git checkout .
```
#### Menyingkirkan perubahan yang tidak masuk status stage pada berkas:
```shell
git checkout {{nama_berkas}}
```
#### Mengganti berkas pada direktori saat ini dengan versi pada cabang lain:
```shell
git checkout {{nama_cabang}} -- {{nama_berkas}}
```
{% endraw %}