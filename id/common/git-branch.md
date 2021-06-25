---
layout: default
title: "git branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-branch">
  <a href="/id/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perintah Git utama untuk bekerja dengan cabang (*branch*).
> Informasi lebih lanjut: <https://git-scm.com/docs/git-branch>.

#### Menampilkan daftar cabang lokal. Cabang saat ini ditandai oleh `*`:
```shell
git branch
```
#### Menampilkan daftar semua cabang (lokal dan remote):
```shell
git branch -a
```
#### Tunjukkan nama cabang saat ini:
```shell
git branch --show-current
```
#### Buat cabang baru berdasarkan komit saat ini:
```shell
git branch {{nama_cabang}}
```
#### Buat cabang baru berdasarkan komit tertentu:
```shell
git branch {{nama_cabang}} {{hash_komit}}
```
#### Ganti nama cabang (harus bukan cabang saat ini untuk melakukannya):
```shell
git branch -m {{nama_cabang_lama}} {{nama_cabang_baru}}
```
#### Hapus cabang lokal (harus bukan cabang saat ini untuk melakukannya):
```shell
git branch -d {{nama_cabang}}
```
#### Hapus cabang remote:
```shell
git push {{nama_remote}} --delete {{nama_cabang_remote}}
```
{% endraw %}