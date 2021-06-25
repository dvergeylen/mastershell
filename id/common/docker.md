---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/id/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengatur kontainer Docker dan image.
> Informasi lebih lanjut: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Menampilkan semua daftar kontainer docker yang sedang berjalan:
```shell
docker ps
```
#### Menampilkan semua daftar kontainer docker (yang sedang berjalan dan berhenti):
```shell
docker ps -a
```
#### Memulai sebuah kontainer dari image, dengan nama kustom:
```shell
docker run --name {{nama_kontainer}} {{image}}
```
#### Memulai atau menghentikan kontainer yang tersedia:
```shell
docker {{start|stop}} {{nama_kontainer}}
```
#### Menarik image dari registri docker:
```shell
docker pull {{image}}
```
#### Membuka shell didalam sebuah kontainer yang sedang berjalan:
```shell
docker exec -it {{nama_kontainer}} {{sh}}
```
#### Menghapus kontainer yang sedang berhenti:
```shell
docker rm {{nama_kontainer}}
```
#### Mengambil dan mengikuti semua log dari sebuah kontainer:
```shell
docker logs -f {{nama_kontainer}}
```
{% endraw %}