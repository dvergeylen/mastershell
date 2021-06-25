---
layout: default
title: "arecord"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arecord">
  <a href="/en/linux/arecord.html">arecord</a> <a href="#arecord"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sound recorder for ALSA soundcard driver.
> More information: <https://manned.org/arecord>.

#### Record a snippet in "CD" quality (finish with Ctrl-C when done):
```shell
arecord -vv --format=cd {{path/to/file.wav}}
```
#### Record a snippet in "CD" quality, with a fixed duration of 10 seconds:
```shell
arecord -vv --format=cd --duration={{10}} {{path/to/file.wav}}
```
#### Record a snippet and save it as mp3 (finish with Ctrl-C when done):
```shell
arecord -vv --format=cd --file-type raw | lame -r - {{path/to/file.mp3}}
```
#### List all sound cards and digital audio devices:
```shell
arecord --list-devices
```
#### Allow interactive interface (e.g. use space-bar or enter to play or pause):
```shell
arecord --interactive
```
{% endraw %}