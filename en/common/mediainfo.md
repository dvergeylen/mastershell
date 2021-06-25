---
layout: default
title: "mediainfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mediainfo">
  <a href="/en/common/mediainfo.html">mediainfo</a> <a href="#mediainfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display metadata from video and audio files.
> More information: <https://mediaarea.net/MediaInfo>.

#### Display metadata for a given file in the console:
```shell
mediainfo {{file}}
```
#### Store the output to a given file along with displaying in the console:
```shell
mediainfo --Logfile={{out.txt}} {{file}}
```
#### Display the list of metadata attributes that can be extracted:
```shell
mediainfo --Info-Parameters
```
{% endraw %}