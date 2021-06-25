---
layout: default
title: "deemix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deemix">
  <a href="/en/common/deemix.html">deemix</a> <a href="#deemix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A barebone deezer downloader library built from the ashes of Deezloader Remix.
> It can be used as a standalone CLI app or implemented in an UI using the API.
> More information: <https://deemix.app>.

#### Download a track or playlist:
```shell
deemix {{https://www.deezer.com/us/track/00000000}}
```
#### Download track / playlist at a specific bitrate:
```shell
deemix --bitrate {{FLAC|MP3}} {{url}}
```
#### Download to a specific path:
```shell
deemix --bitrate {{bitrate}} --path {{path}} {{url}}
```
#### Create a portable deemix config in the current directory:
```shell
deemix --portable --bitrate {{bitrate}} --path {{path}} {{url}}
```
{% endraw %}