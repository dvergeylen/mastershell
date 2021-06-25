---
layout: default
title: "peerflix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="peerflix">
  <a href="/en/common/peerflix.html">peerflix</a> <a href="#peerflix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stream video- or audio-based torrents to a media player.
> More information: <https://github.com/mafintosh/peerflix>.

#### Stream the largest media file in a torrent:
```shell
peerflix "{{torrent_url|magnet_link}}"
```
#### List all streamable files contained in a torrent (given as a magnet link):
```shell
peerflix "{{magnet:?xt=urn:btih:0123456789abcdef0123456789abcdef01234567}}" --list
```
#### Stream the largest file in a torrent, given as a torrent URL, to VLC:
```shell
peerflix "{{http://example.net/music.torrent}}" --vlc
```
#### Stream the largest file in a torrent to MPlayer, with subtitles:
```shell
peerflix "{{torrent_url|magnet_link}}" --mplayer --subtitles {{subtitle-file.srt}}
```
#### Stream all files from a torrent to Airplay:
```shell
peerflix "{{torrent_url|magnet_link}}" --all --airplay
```
{% endraw %}