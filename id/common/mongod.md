---
layout: default
title: "mongod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mongod">
  <a href="/id/common/mongod.html">mongod</a> <a href="#mongod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Server database MongoDB.
> Informasi lebih lanjut: <https://docs.mongodb.com/manual/reference/program/mongod>.

#### Menentukan berkas konfigurasi:
```shell
mongod --config {{nama_berkas}}
```
#### Menentukan port yang digunakan:
```shell
mongod --port {{port}}
```
#### Menentukan tingkat pencatatan perilaku (*profiling*) database. 0 mati, 1 hanya operasi lambat, 2 semuanya:
```shell
mongod --profile {{0|1|2}}
```
{% endraw %}