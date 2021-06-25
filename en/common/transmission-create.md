---
layout: default
title: "transmission-create"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="transmission-create">
  <a href="/en/common/transmission-create.html">transmission-create</a> <a href="#transmission-create"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI utility to create BitTorrent .torrent files.
> More information: <https://manned.org/transmission-create>.

#### Create a torrent with 2048 KB as the piece size:
```shell
transmission-create -o {{path/to/example.torrent}} --tracker {{tracker_announce_url}} --piecesize {{2048}} {{path/to/file_or_directory}}
```
#### Create a private torrent with a 2048 KB piece size:
```shell
transmission-create -p -o {{path/to/example.torrent}} --tracker {{tracker_announce_url}} --piecesize {{2048}} {{path/to/file_or_directory}}
```
#### Create a torrent with a comment:
```shell
transmission-create -o {{path/to/example.torrent}} --tracker {{tracker_url1}} -c {{comment}} {{path/to/file_or_directory}}
```
#### Create a torrent with multiple trackers:
```shell
transmission-create -o {{path/to/example.torrent}} --tracker {{tracker_url1}} --tracker {{tracker_url2}} {{path/to/file_or_directory}}
```
#### Show help page:
```shell
transmission-create --help
```
{% endraw %}