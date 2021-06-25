---
layout: default
title: "git commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit">
  <a href="/id/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komit file ke dalam sebuah repositori.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-commit>.

#### Komit file bertahap ke repositori dengan sebuah pesan:
```shell
git commit -m "{{pesan}}"
```
#### Otomatis merubah semua file yang dimodifikasi menjadi ke status stage dan menambahkan sebuah pesan:
```shell
git commit -a -m "{{pesan}}"
```
#### Ganti komit terakhir dengan perubahan yang ada di status stage saat ini:
```shell
git commit --amend
```
#### Komit file tertentu (yang sudah di status stage):
```shell
git commit {{alamat/ke/file/saya1}} {{alamat/ke/file/saya2}}
```
{% endraw %}