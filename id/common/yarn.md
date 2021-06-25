---
layout: default
title: "yarn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yarn">
  <a href="/id/common/yarn.html">yarn</a> <a href="#yarn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengelola paket alternatif untuk JavaScript dan Node.js.
> Informasi lebih lanjut: <https://yarnpkg.com>.

#### Memasang modul secara global:
```shell
yarn global add {{nama_modul}}
```
#### Memasang semua dependensi yang dirujuk di berkas `package.json` (`install` adalah opsional):
```shell
yarn install
```
#### Memasang modul dan menyimpannya sebagai dependensi ke berkas `package.json` (tambahkan `--dev` untuk menyimpannya sebagai dependensi pengembangan):
```shell
yarn add {{nama_modul}}@{{versi}}
```
#### Mencopot modul dan menghapusnya dari berkas `package.json`:
```shell
yarn remove {{nama_modul}}
```
#### Membuat berkas `package.json` secara interaktif:
```shell
yarn init
```
#### Mengidentifikasi apakah modul merupakan dependensi dan daftar modul lainnya yang bergantung padanya:
```shell
yarn why {{module_name}}
```
{% endraw %}