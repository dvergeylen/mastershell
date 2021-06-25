---
layout: default
title: "alacritty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alacritty">
  <a href="/id/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lintas platform, terakselerasi GPU terminal emulator.
> Informasi lebih lanjut: <https://github.com/alacritty/alacritty>.

#### Membuka jendela Alacritty baru:
```shell
alacritty
```
#### Menjalankan Alacritty pada direktori tertentu:
```shell
alacritty --working-directory {{alamat/ke/direktori}}
```
#### Menjalankan perintah di jendela Alacritty baru:
```shell
alacritty -e {{perintah}}
```
#### Menentukan berkas konfigurasi alternatif (nilai default `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{alamat/ke/konfigurasi.yml}}
```
#### Menjalankan dengan mengaktifkan pemuatan ulang konfigurasi secara langsung/otomatis (dapat juga diaktifkan secara default di `alacritty.yml`):
```shell
alacritty --live-config-reload --config-file {{alamat/ke/konfigurasi.yml}}
```
{% endraw %}