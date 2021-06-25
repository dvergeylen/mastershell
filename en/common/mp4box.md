---
layout: default
title: "mp4box"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mp4box">
  <a href="/en/common/mp4box.html">mp4box</a> <a href="#mp4box"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MPEG-4 Systems Toolbox - Muxes streams into MP4 container.
> More information: <https://gpac.wp.imt.fr/mp4box>.

#### Display information about an existing MP4 file:
```shell
mp4box -info {{filename}}
```
#### Add an SRT subtitle file into an MP4 file:
```shell
mp4box -add {{input_subs.srt}}:lang=eng -add {{input.mp4}} {{output.mp4}}
```
#### Combine audio from one file and video from another:
```shell
mp4box -add {{input1.mp4}}#audio -add {{input2.mp4}}#video {{output.mp4}}
```
{% endraw %}