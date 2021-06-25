---
layout: default
title: "mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mv">
  <a href="/id/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Memindah atau menamai-ulang file dan direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/mv>.

#### Memindahkan file ke lokasi yang baru:
```shell
mv {{sumber}} {{tujuan}}
```
#### Memindah tanpa meminta konfirmasi sebelum menimpa file yang sudah ada:
```shell
mv -f {{sumber}} {{tujuan}}
```
#### Meminta konfirmasi sebelum menimpa file yang sudah ada, apapun *file permissions*-nya:
```shell
mv -i {{sumber}} {{tujuan}}
```
#### Jangan menimpa file yang sudah ada di direktori tujuan:
```shell
mv -n {{sumber}} {{tujuan}}
```
#### Memindahkan file dalam mode *verbose*, menampilkan file-file yang dipindahkan:
```shell
mv -v {{sumber}} {{tujuan}}
```
{% endraw %}