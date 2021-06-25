---
layout: default
title: "vue init"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vue-init">
  <a href="/id/common/vue-init.html">vue init</a> <a href="#vue-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sub-perintah untuk menginisialisasi proyek warisan framework Vue.js.
> Informasi lebih lanjut: <https://cli.vuejs.org/guide/creating-a-project.html#pulling-2-x-templates-legacy>.

#### Buat proyek baru dengan menggunakan salah satu templat bawaan:
```shell
vue init {{webpack|webpack-simple|browserify|browserify-simple|simple}} {{nama_proyek}}
```
#### Buat proyek baru menggunakan templat lokal:
```shell
vue init {{lokasi/ke/templat_direktori}} {{nama_proyek}}
```
#### Buat proyek baru dengan menggunakan templat dari GitHub:
```shell
vue init {{username}}/{{repo}} {{nama_proyek}}
```
{% endraw %}