---
layout: default
title: "deluge-console"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluge-console">
  <a href="/en/common/deluge-console.html">deluge-console</a> <a href="#deluge-console"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive interface for the Deluge BitTorrent client.
> More information: <https://deluge-torrent.org>.

#### Start the interactive console interface:
```shell
deluge-console
```
#### Connect to a Deluge daemon instance:
```shell
connect {{hostname}}:{{port}}
```
#### Add a torrent to the daemon:
```shell
add {{url|magnet|path/to/file}}
```
#### Display information about all torrents:
```shell
info
```
#### Display information about a specific torrent:
```shell
info {{torrent_id}}
```
#### Pause a torrent:
```shell
pause {{torrent_id}}
```
#### Resume a torrent:
```shell
resume {{torrent_id}}
```
#### Remove a torrent from the daemon:
```shell
rm {{torrent_id}}
```
{% endraw %}