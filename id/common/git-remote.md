---
layout: default
title: "git remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-remote">
  <a href="/id/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengelola kumpulan repositori yang dilacak/diikuti ("remotes").
> Informasi lebih lanjut: <https://git-scm.com/docs/git-remote>.

#### Menampilkan daftar remote, namanya dan URL:
```shell
git remote -v
```
#### Menampilkan informasi tentang remote:
```shell
git remote show {{nama_remote}}
```
#### Menambahkan remote:
```shell
git remote add {{nama_remote}} {{url_remote}}
```
#### Mengubah URL dari remote (gunakan `--add` untuk tetap menyimpan URL lama):
```shell
git remote set-url {{nama_remote}} {{url_baru}}
```
#### Menghapus remote:
```shell
git remote remove {{nama_remote}}
```
#### Mengubah nama remote:
```shell
git remote rename {{nama_lama}} {{nama_baru}}
```
{% endraw %}