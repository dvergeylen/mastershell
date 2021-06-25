---
layout: default
title: "spotify"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="spotify">
  <a href="/en/osx/spotify.html">spotify</a> <a href="#spotify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface to Spotify.
> More information: <https://github.com/hnarayanan/shpotify>.

#### Find a song by name and play it:
```shell
spotify play {{song_name}}
```
#### Find a playlist by name and play it:
```shell
spotify play list {{playlist_name}}
```
#### Pause (or resume) playback:
```shell
spotify pause
```
#### Skip to the next song in a playlist:
```shell
spotify next
```
#### Change volume:
```shell
spotify vol {{up|down|value}}
```
#### Show the playback status and song details:
```shell
spotify status
```
{% endraw %}