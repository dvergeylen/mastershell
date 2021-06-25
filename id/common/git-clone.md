---
layout: default
title: "git clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clone">
  <a href="/id/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengkloning repositori yang ada.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-clone>.

#### Mengkloning repositori yang ada:
```shell
git clone {{lokasi_repositori_remote}}
```
#### Mengkloning reposiori yang ada dan submodulenya:
```shell
git clone --recursive {{lokasi_repositori_remote}}
```
#### Mengkloning repositori lokal:
```shell
git clone -l {{alamat/ke/repository/lokal}}
```
#### Mengkloning dengan senyap:
```shell
git clone -q {{lokasi_repositori_remote}}
```
#### Mengkloning repositori yang sudah ada dengan hanya mengambil 10 komit paling baru pada branch default (berguna untuk menghemat waktu):
```shell
git clone --depth {{10}} {{lokasi_repositori_remote}}
```
{% endraw %}