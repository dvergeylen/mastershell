---
layout: default
title: "wacaw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wacaw">
  <a href="/en/osx/wacaw.html">wacaw</a> <a href="#wacaw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A little command-line tool for macOS that allows you to capture both still pictures and video from an attached camera.
> More information: <http://webcam-tools.sourceforge.net>.

#### Take a picture from webcam:
```shell
wacaw {{filename}}
```
#### Record a video:
```shell
wacaw --video {{filename}} -D {{duration_in_seconds}}
```
#### Take a picture with custom resolution:
```shell
wacaw -x {{width}} -y {{height}} {{filename}}
```
#### Copy image just taken to clipboard:
```shell
wacaw --to-clipboard
```
#### List the devices available:
```shell
wacaw -L
```
{% endraw %}