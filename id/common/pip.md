---
layout: default
title: "pip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pip">
  <a href="/id/common/pip.html">pip</a> <a href="#pip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengelola paket Python.
> Informasi lebih lanjut: <https://pip.pypa.io>.

#### Memasang paket:
```shell
pip install {{nama_paket}}
```
#### Memasang versi paket tertentu:
```shell
pip install {{nama_paket}}=={{versi_paket}}
```
#### Meningkatakan paket ke versi terbaru:
```shell
pip install -U {{nama_paket}}
```
#### Mencopot pemasangan paket:
```shell
pip uninstall {{nama_paket}}
```
#### Menyimpan daftar paket terpasang ke berkas:
```shell
pip freeze > {{requirements.txt}}
```
#### Memasang paket dari berkas:
```shell
pip install -r {{requirements.txt}}
```
#### Menampilkan informasi paket terpasang:
```shell
pip show {{nama_paket}}
```
{% endraw %}