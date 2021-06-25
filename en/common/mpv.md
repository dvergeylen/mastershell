---
layout: default
title: "mpv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mpv">
  <a href="/en/common/mpv.html">mpv</a> <a href="#mpv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A audio/video player based on MPlayer.
> More information: <https://mpv.io>.

#### Play a video or audio file:
```shell
mpv {{file}}
```
#### Play a video or audio file from an URL:
```shell
mpv '{{https://www.youtube.com/watch?v=dQw4w9WgXcQ}}'
```
#### Jump backward/forward 5 seconds:
```shell
LEFT <or> RIGHT
```
#### Jump backward/forward 1 minute:
```shell
DOWN <or> UP
```
#### Decrease or increase playback speed by 10 %:
```shell
[ <or> ]
```
#### Play a file at a specified speed (0.01 to 100, default 1):
```shell
mpv --speed {{speed}} {{file}}
```
#### Play a file using a profile defined in the `mpv.conf` file:
```shell
mpv --profile {{profile_name}} {{file}}
```
#### Display the output of webcam or other video input device:
```shell
mpv /dev/{{video0}}
```
{% endraw %}