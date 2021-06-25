---
layout: default
title: "mkvmerge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkvmerge">
  <a href="/en/common/mkvmerge.html">mkvmerge</a> <a href="#mkvmerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Merge and extract multimedia streams.
> More information: <https://mkvtoolnix.download/doc/mkvmerge.html>.

#### Display information about a Matroska file:
```shell
mkvmerge --identify {{path/to/file.mkv}}
```
#### Extract the audio from track 1 of a specific file:
```shell
mkvextract tracks {{path/to/file.mkv}} {{1}}:{{path/to/output.webm}}
```
#### Extract the subtitle from track 3 of a specific file:
```shell
mkvextract tracks {{path/to/file.mkv}} {{3}}:{{path/to/subs.srt}}
```
{% endraw %}