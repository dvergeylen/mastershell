---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/id/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Membuat alias -- kata-kata yang digantikan oleh utasan perintah (command).
> Alias menjadi kadaluarsa sampai sesi shell saat ini berakhir, kecuali jika didefinisikan di file konfigurasi shell, misalnya `~/.bashrc`.
> Informasi lebih lanjut: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Menampilkan daftar semua alias:
```shell
alias
```
#### Membuat alias generik:
```shell
alias {{kata}}="{{perintah}}"
```
#### Melihat perintah yang dirujuk oleh alias yang diberikan:
```shell
alias {{kata}}
```
#### Menghapus alias dari sebuah perintah:
```shell
unalias {{kata}}
```
#### Mengubah `rm` menjadi perintah interaktif:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Membuat `la` menjadi pintasan untuk `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}