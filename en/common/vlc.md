---
layout: default
title: "vlc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vlc">
  <a href="/en/common/vlc.html">vlc</a> <a href="#vlc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cross-platform multimedia player.
> More information: <https://www.videolan.org/vlc/>.

#### Play a file:
```shell
vlc {{path/to/file}}
```
#### Play in fullscreen:
```shell
vlc --fullscreen {{path/to/file}}
```
#### Play muted:
```shell
vlc --no-audio {{path/to/file}}
```
#### Play repeatedly:
```shell
vlc --loop {{path/to/file}}
```
#### Play video from a URL:
```shell
vlc {{https://www.youtube.com/watch?v=oHg5SJYRHA0}}
```
{% endraw %}