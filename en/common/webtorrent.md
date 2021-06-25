---
layout: default
title: "webtorrent"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="webtorrent">
  <a href="/en/common/webtorrent.html">webtorrent</a> <a href="#webtorrent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The command-line interface for WebTorrent.
> Supports magnets, urls, info hashes and .torrent files.
> More information: <https://github.com/webtorrent/webtorrent-cli>.

#### Download a torrent:
```shell
webtorrent download "{{torrent_id}}"
```
#### Stream a torrent to VLC media player:
```shell
webtorrent download "{{torrent_id}}" --vlc
```
#### Stream a torrent to a Digital Living Network Alliance (DLNA) device:
```shell
webtorrent download "{{torrent_id}}" --dlna
```
#### Display a list of files for a specific torrent:
```shell
webtorrent download "{{torrent_id}}" --select
```
#### Specify a file index from the torrent to download:
```shell
webtorrent download "{{torrent_id}}" --select {{index}}
```
#### Seed a specific file or directory:
```shell
webtorrent seed {{path/to/file_or_directory}}
```
#### Create a new torrent file for the specified file path:
```shell
webtorrent create {{path/to/file}}
```
#### Display information for a magnet URI or `.torrent` file:
```shell
webtorrent info {{path/to/file_or_magnet}}
```
{% endraw %}