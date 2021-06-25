---
layout: default
title: "dir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dir">
  <a href="/id/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lis isi direktori.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### Tampilkan isi direktori saat ini:
```shell
dir
```
#### Tampilkan isi direktori yang ditentukan:
```shell
dir {{lokasi/ke/direktori}}
```
#### Tampilkan isi dari direktori saat ini, termasuk yang disembunyikan:
```shell
dir /A
```
#### Tampilkan isi direktori yang ditentukan, termasuk yang disembunyikan:
```shell
dir {{lokasi/ke/direktori}} /A
```
{% endraw %}