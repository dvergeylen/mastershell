---
layout: default
title: "transcode"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="transcode">
  <a href="/en/common/transcode.html">transcode</a> <a href="#transcode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transcode video and audio codecs, and convert between media formats.

#### Create stabilisation file to be able to remove camera shakes:
```shell
transcode -J stabilize -i {{input_file}}
```
#### Remove camera shakes after creating stabilisation file, transform video using xvid:
```shell
transcode -J transform -i {{input_file}} -y xvid -o {{output_file}}
```
#### Resize the video to 640x480 pixels and convert to MPEG4 codec using xvid:
```shell
transcode -Z 640x480 -i {{input_file}} -y xvid -o {{output_file}}
```
{% endraw %}