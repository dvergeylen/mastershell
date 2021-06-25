---
layout: default
title: "id3tag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="id3tag">
  <a href="/en/common/id3tag.html">id3tag</a> <a href="#id3tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for reading, writing, and manipulating ID3v1 and ID3v2 tags of MP3 files.

#### Set artist and title tag of an MP3 file:
```shell
id3tag --artist={{artist}} --title={{title}} {{path/to/file.mp3}}
```
#### Set album title of all MP3 files in the current directory:
```shell
id3tag --album={{album}} {{*.mp3}}
```
#### Get more help:
```shell
id3tag --help
```
{% endraw %}