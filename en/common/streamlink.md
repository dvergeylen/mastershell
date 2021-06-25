---
layout: default
title: "streamlink"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="streamlink">
  <a href="/en/common/streamlink.html">streamlink</a> <a href="#streamlink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extracts streams from various services and pipes them into a video player of choice.
> More information: <https://streamlink.github.io>.

#### Attempt to extract streams from the URL specified, and if it's successful, print out a list of available streams to choose from:
```shell
streamlink {{example.com/stream}}
```
#### Open a stream with the specified quality:
```shell
streamlink {{example.com/stream}} {{720p60}}
```
#### Select the highest or lowest available quality:
```shell
streamlink {{example.com/stream}} {{best|worst}}
```
#### Specify which player to use to feed stream data to (VLC is used by default if found):
```shell
streamlink --player={{mpv}} {{example.com/stream}} {{best}}
```
#### Specify the amount of time to skip from the beginning of the stream. For live streams, this is a negative offset from the end of the stream (rewind):
```shell
streamlink --hls-start-offset {{[HH:]MM:SS}} {{example.com/stream}} {{best}}
```
#### Skip to the beginning of a live stream, or as far back as possible:
```shell
streamlink --hls-live-restart {{example.com/stream}} {{best}}
```
#### Write stream data to a file instead of playing it:
```shell
streamlink --output {{path/to/file.ts}} {{example.com/stream}} {{best}}
```
#### Open the stream in the player, while at the same time writing it to a file:
```shell
streamlink --record {{path/to/file.ts}} {{example.com/stream}} {{best}}
```
{% endraw %}