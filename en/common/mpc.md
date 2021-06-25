---
layout: default
title: "mpc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mpc">
  <a href="/en/common/mpc.html">mpc</a> <a href="#mpc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Music Player Client.
> Program for controlling the Music Player Daemon (MPD).
> More information: <https://www.musicpd.org/clients/mpc>.

#### Toggle play/pause:
```shell
mpc toggle
```
#### Stop playing:
```shell
mpc stop
```
#### Show information about the currently playing song:
```shell
mpc status
```
#### Play next song:
```shell
mpc next
```
#### Play previous song:
```shell
mpc prev
```
#### Forward or rewind the currently playing song:
```shell
mpc [+-]{{seconds}}
```
{% endraw %}