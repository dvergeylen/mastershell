---
layout: default
title: "transmission-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="transmission-cli">
  <a href="/en/common/transmission-cli.html">transmission-cli</a> <a href="#transmission-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A lightweight, command-line BitTorrent client.
> This tool has been deprecated, please see `transmission-remote`.
> More information: <https://transmissionbt.com>.

#### Download a specific torrent:
```shell
transmission-cli {{url|magnet|path/to/file}}
```
#### Download a torrent to a specific directory:
```shell
transmission-cli --download-dir {{path/to/download_directory}} {{url|magnet|path/to/file}}
```
#### Create a torrent file from a specific file or directory:
```shell
transmission-cli --new {{path/to/source_file_or_directory}}
```
#### Set the download speed limit to 50 KB/s:
```shell
transmission-cli --downlimit {{50}} {{url|magnet|path/to/file}}
```
#### Set the upload speed limit to 50 KB/s:
```shell
transmission-cli --uplimit {{50}} {{url|magnet|path/to/file}}
```
#### Use a specific port for connections:
```shell
transmission-cli --port {{port_number}} {{url|magnet|path/to/file}}
```
#### Force encryption for peer connections:
```shell
transmission-cli --encryption-required {{url|magnet|path/to/file}}
```
#### Use a Bluetack-formatted peer blocklist:
```shell
transmission-cli --blocklist {{blocklist_url|path/to/blocklist}} {{url|magnet|path/to/file}}
```
{% endraw %}