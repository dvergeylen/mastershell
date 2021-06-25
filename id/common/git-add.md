---
layout: default
title: "git add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-add">
  <a href="/id/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menambahkan file yang diubah ke indeks.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-add>.

#### Tambahkan file ke indeks:
```shell
git add {{alamat/ke/file}}
```
#### Tambahkan semua file (yang terlacak dan tidak terlacak):
```shell
git add -A
```
#### Hanya tambahkan file yang sudah terlacak:
```shell
git add -u
```
#### Tambahkan juga file yang diabaikan:
```shell
git add -f
```
#### Menambahkan file ke status stage secara interaktif:
```shell
git add -p
```
#### Menambahkan file tertentu ke status stage secara interaktif:
```shell
git add -p {{alamat/ke/file}}
```
#### Stage file secara interaktif:
```shell
git add -i
```
{% endraw %}