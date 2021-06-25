---
layout: default
title: "find"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="find">
  <a href="/id/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mencari teks tertentu di dalam suatu file atau direktori.
> Informasi lebih lanjut: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### Mencari baris-baris dalam file yang mengandung teks tertentu:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}}
```
#### Menunjukkan baris-baris dalam file yang tidak mengandung teks tertentu:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}} /v
```
#### Menghitung jumlah baris dalam file yang mengandung teks tertentu:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}} /c
```
#### Mencari baris-baris dalam file yang mengandung teks tertentu beserta nomor barisnya:
```shell
find {{teks}} {{jalan/menuju/file_atau_direktori}} /n
```
{% endraw %}