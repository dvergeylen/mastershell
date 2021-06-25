---
layout: default
title: "transmission-remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="transmission-remote">
  <a href="/en/common/transmission-remote.html">transmission-remote</a> <a href="#transmission-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remote control utility for transmission-daemon and transmission.
> More information: <https://transmissionbt.com>.

#### Add a torrent file or magnet link to Transmission and download to a specified directory:
```shell
transmission-remote {{hostname}} -a {{torrent|url}} -w {{/path/to/download_directory}}
```
#### Change the default download directory:
```shell
transmission-remote {{hostname}} -w {{/path/to/download_directory}}
```
#### List all torrents:
```shell
transmission-remote {{hostname}} --list
```
#### Start torrent 1 and 2, stop torrent 3:
```shell
transmission-remote {{hostname}} -t "{{1,2}}" --start -t {{3}} --stop
```
#### Remove torrent 1 and 2, and also delete local data for torrent 2:
```shell
transmission-remote {{hostname}} -t {{1}} --remove -t {{2}} --remove-and-delete
```
#### Stop all torrents:
```shell
transmission-remote {{hostname}} -t {{all}} --stop
```
#### Move torrents 1-10 and 15-20 to a new directory (which will be created if it does not exist):
```shell
transmission-remote {{hostname}} -t "{{1-10,15-20}}" --move {{/path/to/new_directory}}
```
{% endraw %}