---
layout: default
title: "java"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="java">
  <a href="/id/common/java.html">java</a> <a href="#java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Peluncur Aplikasi Java.
> Informasi lebih lanjut: <https://java.com>.

#### Menjalankan berkas java `.class` yang mengandung method main dengan hanya menggunakan nama class:
```shell
java {{nama_class}}
```
#### Menjalankan program `.jar`:
```shell
java -jar {{nama_berkas.jar}}
```
#### Menjalankan program `.jar` dengan menunggu debugger terhubung ke port 5005:
```shell
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{nama_berkas.jar}}
```
#### Menampilkan versi JDK, JRE dan HotSpot:
```shell
java -version
```
#### Menampilkan informasi penggunaan untuk perintah java:
```shell
java -help
```
{% endraw %}