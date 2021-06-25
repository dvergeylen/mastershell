---
layout: default
title: "fswebcam"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fswebcam">
  <a href="/en/common/fswebcam.html">fswebcam</a> <a href="#fswebcam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Small and simple webcam for *nix.
> More information: <https://www.sanslogic.co.uk/fswebcam>.

#### Take a picture:
```shell
fswebcam {{filename}}
```
#### Take a picture with custom resolution:
```shell
fswebcam -r {{width}}x{{height}} {{filename}}
```
#### Take a picture from selected device(Default is `/dev/video0`):
```shell
fswebcam -d {{device}} {{filename}}
```
#### Take a picture with timestamp(timestamp string is formatted by strftime):
```shell
fswebcam --timestamp {{timestamp}} {{filename}}
```
{% endraw %}