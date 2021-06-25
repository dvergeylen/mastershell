---
layout: default
title: "eyeD3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eyed3">
  <a href="/en/linux/eyed3.html">eyeD3</a> <a href="#eyed3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read and manipulate metadata of MP3 files.
> More information: <https://eyed3.readthedocs.io/en/latest/>.

#### View information about an MP3 file:
```shell
eyeD3 {{filename.mp3}}
```
#### Set the title of an MP3 file:
```shell
eyeD3 --title "{{A Title}}" {{filename.mp3}}
```
#### Set the album of all the MP3 files in a directory:
```shell
eyeD3 --album "{{Album Name}}" {{*.mp3}}
```
#### Set the front cover art for an MP3 file:
```shell
eyeD3 --add-image {{front_cover.jpeg}}:FRONT_COVER: {{filename.mp3}}
```
{% endraw %}