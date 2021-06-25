---
layout: default
title: "git"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git">
  <a href="/id/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sistem kontrol versi terdistribusi.
> Informasi lebih lanjut: <https://git-scm.com/>.

#### Memeriksa versi Git:
```shell
git --version
```
#### Menunjukkan bantuan umum:
```shell
git --help
```
#### Menampilkan bantuan pada sub perintah Git (seperti `commit`,` log`, dll.):
```shell
git help {{subcommand}}
```
#### Menjalankan subperintah Git:
```shell
git {{subcommand}}
```
#### Menjalankan subperintah Git di jalur root repositori kustom:
```shell
git -C {{alamat/ke/repositori}} {{subcommand}}
```
#### Menjalankan subperintah Git dengan set konfigurasi yang diberikan:
```shell
git -c '{{config.key}}={{value}}' {{subcommand}}
```
{% endraw %}