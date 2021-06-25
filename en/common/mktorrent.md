---
layout: default
title: "mktorrent"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mktorrent">
  <a href="/en/common/mktorrent.html">mktorrent</a> <a href="#mktorrent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI utility to create BitTorrent metainfo files.
> More information: <https://github.com/Rudde/mktorrent>.

#### Create a torrent with 2^21 KB as the piece size:
```shell
mktorrent -a {{tracker_announce_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}
```
#### Create a private torrent with a 2^21 KB piece size:
```shell
mktorrent -p -a {{tracker_announce_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}
```
#### Create a torrent with a comment:
```shell
mktorrent -c "{{comment}}" -a {{tracker_announce_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}
```
#### Create a torrent with multiple trackers:
```shell
mktorrent -a {{tracker_announce_url,tracker_announce_url_2}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}
```
#### Create a torrent with web seed URLs:
```shell
mktorrent -a {{tracker_announce_url}} -w {{web_seed_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}
```
{% endraw %}