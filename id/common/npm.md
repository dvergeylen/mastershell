---
layout: default
title: "npm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="npm">
  <a href="/id/common/npm.html">npm</a> <a href="#npm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manajer paket JavaScript dan Node.js.
> Mengelola proyek Node.js dan dependensi modulnya.
> Informasi lebih lanjut: <https://www.npmjs.com/>.

#### Membuat file `package.json` secara interaktif:
```shell
npm init
```
#### Unduh semua paket yang terdaftar sebagai dependensi di package.json:
```shell
npm install
```
#### Unduh versi tertentu dari sebuah paket dan menambahkan ke daftar dependensi di `package.json`:
```shell
npm install {{nama_modul}}@{{versi}}
```
#### Unduh paket dan menambahkan ke daftar dependensi dev di package.json:
```shell
npm install {{nama_modul}} --save-dev
```
#### Unduh paket dan instal secara global:
```shell
npm install --global {{nama_modul}}
```
#### Copot pemasangan paket dan hapus dari daftar dependensi di `package.json`:
```shell
npm uninstall {{nama_modul}}
```
#### Mencetak pohon dependensi yang diinstal secara lokal:
```shell
npm list
```
#### Buat daftar modul tingkat atas yang diinstal secara global:
```shell
npm list --global --depth={{0}}
```
{% endraw %}