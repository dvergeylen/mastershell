---
layout: default
title: "deluge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluge">
  <a href="/en/common/deluge.html">deluge</a> <a href="#deluge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line BitTorrent client.
> More information: <https://deluge-torrent.org>.

#### Download a torrent:
```shell
deluge {{url|magnet|path/to/file}}
```
#### Download a torrent using a specific configuration file:
```shell
deluge -c {{path/to/configuration_file}} {{url|magnet|path/to/file}}
```
#### Download a torrent and launch the specified user interface:
```shell
deluge -u {{gtk|web|console}} {{url|magnet|path/to/file}}
```
#### Download a torrent and output the log to a file:
```shell
deluge -l {{path/to/log_file}} {{url|magnet|path/to/file}}
```
{% endraw %}