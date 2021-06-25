---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cd">
  <a href="/id/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan nama atau ganti direktori saat ini.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Menuju suatu direktori pada drive yang sama:
```shell
cd {{lokasi/ke/direktori}}
```
#### Menampilkan nama dari direktori saat ini:
```shell
cd
```
#### Menuju ke induk direktori dari direktori saat ini:
```shell
cd ..
```
#### Menuju direktori di dalam suatu drive:
```shell
cd {{lokasi/ke/direktori}} /d
```
{% endraw %}