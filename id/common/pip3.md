---
layout: default
title: "pip3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pip3">
  <a href="/id/common/pip3.html">pip3</a> <a href="#pip3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengelola paket Python.
> Informasi lebih lanjut: <https://pip.pypa.io>.

#### Menemukan paket tersedia:
```shell
pip3 search {{nama_paket}}
```
#### Memasang paket:
```shell
pip3 install {{nama_paket}}
```
#### Memasang versi paket tertentu:
```shell
pip3 install {{nama_paket}}=={{versi_paket}}
```
#### Meningkatkan paket ke versi terbaru:
```shell
pip3 install --upgrade {{nama_paket}}
```
#### Mencopot pemasangan paket:
```shell
pip3 uninstall {{nama_paket}}
```
#### Menyimpan daftar paket terpasang ke berkas:
```shell
pip3 freeze > {{requirements.txt}}
```
#### Memasang paket dari berkas:
```shell
pip3 install --requirement {{requirements.txt}}
```
#### Menampilkan informasi paket terinstal:
```shell
pip3 show {{nama_paket}}
```
{% endraw %}