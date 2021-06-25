---
layout: default
title: "youtube-viewer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="youtube-viewer">
  <a href="/en/common/youtube-viewer.html">youtube-viewer</a> <a href="#youtube-viewer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line application for searching and playing videos from YouTube.
> More information: <https://github.com/trizen/youtube-viewer>.

#### Search for a video:
```shell
youtube-viewer {{search_term}}
```
#### Log in to your YouTube account:
```shell
youtube-viewer --login
```
#### Watch a video with a specific URL in VLC:
```shell
youtube-viewer --player={{vlc}} {{https://youtube.com/watch?v=dQw4w9WgXcQ}}
```
#### Display a search prompt and play the selected video in 720p:
```shell
youtube-viewer -{{7}}
```
{% endraw %}