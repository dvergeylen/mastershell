---
layout: default
title: "git status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-status">
  <a href="/id/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan perubahan pada file dalam repositori Git.
> Menmapilkan daftar perubahan , menambahkan dan menghapus file dibandingkan dengan komit yang saat ini di check-out.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-status>.

#### Tampilkan file yang diubah yang belum ditambahkan untuk komit:
```shell
git status
```
#### Berikan keluaran dalam format [s]hort (pendek):
```shell
git status -s
```
#### Jangan tampilkan file yang tidak terlacak di output:
```shell
git status --untracked-files=no
```
#### Tampilkan keluaran dalam format [s]hort (pendek) bersama dengan [b] info cabangnya:
```shell
git status -sb
```
{% endraw %}