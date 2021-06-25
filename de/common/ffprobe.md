---
layout: default
title: "ffprobe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ffprobe">
  <a href="/de/common/ffprobe.html">ffprobe</a> <a href="#ffprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multimedia Stream Analysierer.
> Weitere Informationen: <https://ffmpeg.org/ffprobe.html>.

#### Zeige alle verfügbaren Stream-Informationen einer Medien-Datei an:
```shell
ffprobe -v error -show_entries {{datei.mp4}}
```
#### Zeige Spieldauer an:
```shell
ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
#### Zeige die Bildfrequenz eines Videos an:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream=avg_frame_rate -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
#### Zeige die Breite (width) oder Höhe (height) eines Videos an:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream={{width|height}} -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
#### Zeige die durchschnittliche Bitrate eines Videos an:
```shell
ffprobe -v error -select_streams v:0 -show_entries stream=bit_rate -of default=noprint_wrappers=1:nokey=1 {{datei.mp4}}
```
{% endraw %}