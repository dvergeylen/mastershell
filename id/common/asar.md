---
layout: default
title: "asar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asar">
  <a href="/id/common/asar.html">asar</a> <a href="#asar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengarsip berkas untuk platform Electron.
> Informasi lebih lanjut: <https://github.com/electron/asar>.

#### Arsipkan sebuah berkas atau direktori:
```shell
asar pack {{alamat/ke/berkas_atau_direktori}} {{arsip.asar}}
```
#### Mengekstrak sebuah arsip:
```shell
asar extract {{arsip.asar}}
```
#### Mengekstrak berkas tertentu dari sebuah arsip:
```shell
asar extract-file {{arsip.asar}} {berkas}}
```
#### Mendapatkan daftar konten dari berkas arsip:
```shell
asar list {{arsip.asar}}
```
{% endraw %}