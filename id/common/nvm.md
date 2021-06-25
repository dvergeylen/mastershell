---
layout: default
title: "nvm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nvm">
  <a href="/id/common/nvm.html">nvm</a> <a href="#nvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Memasang, melepas, atau mengganti versi Node.js yang dipakai.
> Mendukung nomor versi seperti "0.12" or "v4.2", dan label versi seperti "stable", "system", dsb.
> Informasi lebih lanjut: <https://github.com/creationix/nvm>.

#### Memasang versi Node.js yang ditentukan:
```shell
nvm install {{versi_node_js}}
```
#### Menggunakan versi Node.js tertentu untuk sesi saat ini:
```shell
nvm use {{versi_node_js}}
```
#### Menyetel versi Node.js secara default:
```shell
nvm alias default {{versi_node_js}}
```
#### Menunjukkan daftar versi Node.js yang tersedia dan versi Node.js yang disetel sebagai default:
```shell
nvm list
```
#### Menghapus sebuah versi Node.js yang terpasang melalui `nvm`:
```shell
nvm uninstall {{versi_node_js}}
```
#### Menjalankan interpreter (REPL) Node.js dengan versi tertentu:
```shell
nvm run {{versi_node_js}} --version
```
#### Menjalankan sebuah file atau aplikasi JavaScript di dalam Node.js versi tertentu:
```shell
nvm exec {{versi_node_js}} node {{app.js}}
```
{% endraw %}