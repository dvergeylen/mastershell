---
layout: default
title: "chkdsk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chkdsk">
  <a href="/id/windows/chkdsk.html">chkdsk</a> <a href="#chkdsk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Memeriksa dan mencari kesalahan dalam sebuah sistem file dan metadata volume penyimpanan.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/chkdsk>.

#### Memeriksa sebuah ruang penyimpanan berdasarkan huruf drive (diakhiri dengan titik dua), lokasi pemasangan, atau nama ruang:
```shell
chkdsk {{ruang_penyimpanan}}
```
#### Memperbaiki kesalahan pada ruang penyimpanan yang ditentukan:
```shell
chkdsk {{ruang_penyimpanan}} /f
```
#### Melepas ruang penyimpanan tertentu untuk pemeriksaan:
```shell
chkdsk {{ruang_penyimpanan}} /x
```
#### Mengubah ukuran file log dalam sebuah ruang penyimpanan dengan sistem file NTFS:
```shell
chkdsk /l{{ukuran}}
```
{% endraw %}