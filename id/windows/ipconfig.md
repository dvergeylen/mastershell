---
layout: default
title: "ipconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipconfig">
  <a href="/id/windows/ipconfig.html">ipconfig</a> <a href="#ipconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan dan mengatur konfigurasi jaringan dalam sistem operasi Windows.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/ipconfig>.

#### Menunjukkan daftar adaptor jaringan:
```shell
ipconfig
```
#### Menunjukkan daftar adaptor jaringan secara lengkap:
```shell
ipconfig /all
```
#### Memperbarui alamat IP sebuah adaptor jaringan:
```shell
ipconfig /renew {{adaptor}}
```
#### Mengosongkan alamat-alamat IP yang disetel dalam sebuah adaptor jaringan:
```shell
ipconfig /release {{adaptor}}
```
#### Mengosongkan cache DNS:
```shell
ipconfig /flushdns
```
{% endraw %}