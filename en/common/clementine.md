---
layout: default
title: "clementine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clementine">
  <a href="/en/common/clementine.html">clementine</a> <a href="#clementine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A modern music player and library organizer.
> More information: <https://www.clementine-player.org>.

#### Open Clementine:
```shell
clementine
```
#### Start playing a music file:
```shell
clementine {{url/or/path/to/file.ext}}
```
#### Toggle between pausing and playing:
```shell
clementine --play-pause
```
#### Stop playback:
```shell
clementine --stop
```
#### Skip to the next track:
```shell
clementine --next
```
#### Skip to the previous track:
```shell
clementine --previous
```
#### Load a playlist file:
```shell
clementine --load {{path/to/playlist.ext}}
```
#### Play the 5th track in the currently loaded playlist:
```shell
clementine --play-track {{5}}
```
{% endraw %}