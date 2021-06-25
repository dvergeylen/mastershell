---
layout: default
title: "ffprobe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ffprobe">
  <a href="/en/common/ffprobe.html">ffprobe</a> <a href="#ffprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multimedia stream analyzer.
> More information: <https://ffmpeg.org/ffprobe.html>.

#### Display all available stream info for a media file:
```shell
ffprobe -v error -show_entries {{input.mp4}}
```
#### Display media duration:
```shell
ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}
```
#### Display the frame rate of a video:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream=avg_frame_rate -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}
```
#### Display the width or height of a video:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream={{width|height}} -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}
```
#### Display the average bit rate of a video:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream=bit_rate -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}
```
{% endraw %}