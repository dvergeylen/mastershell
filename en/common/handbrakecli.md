---
layout: default
title: "handbrakecli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="handbrakecli">
  <a href="/en/common/handbrakecli.html">handbrakecli</a> <a href="#handbrakecli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface to the HandBrake video conversion tool.
> More information: <https://handbrake.fr/>.

#### Convert a video file to MKV (AAC 160kbit audio and x264 CRF20 video):
```shell
handbrakecli -i {{input.avi}} -o {{output.mkv}} -e x264 -q 20 -B 160
```
#### Resize a video file to 320x240:
```shell
handbrakecli -i {{input.mp4}} -o {{output.mp4}} -w 320 -l 240
```
#### List available presets:
```shell
handbrakecli --preset-list
```
#### Convert an AVI video to MP4 using the Android preset:
```shell
handbrakecli --preset="Android" -i {{input.ext}} -o {{output.mp4}}
```
{% endraw %}