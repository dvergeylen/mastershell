---
layout: default
title: "laravel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="laravel">
  <a href="/id/common/laravel.html">laravel</a> <a href="#laravel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pemasang Laravel framework berbasis command-line.
> Informasi lebih lanjut: <https://laravel.com>.

#### Buat aplikasi Laravel baru:
```shell
laravel new {{nama}}
```
#### Gunakan versi pengembangan terkini:
```shell
laravel new {{nama}} --dev
```
#### Overwrite if the directory already exists:
```shell
laravel new {{nama}} --force
```
#### Pasang struktur Laravel Jetstream:
```shell
laravel new {{nama}} --jet
```
#### Pasang struktur Laravel Jetstream dengan susunan tertentu:
```shell
laravel new {{nama}} --jet --stack {{livewire|inertia}}
```
#### Pasang struktur Laravel Jetstream dengan dukungan tim:
```shell
laravel new {{nama}} --jet --teams
```
#### Lis perintah yang tersedia:
```shell
laravel list
```
{% endraw %}