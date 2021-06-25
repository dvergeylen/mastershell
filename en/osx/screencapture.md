---
layout: default
title: "screencapture"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="screencapture">
  <a href="/en/osx/screencapture.html">screencapture</a> <a href="#screencapture"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to take screenshots and screen recordings.

#### Take a screenshot and save it to a file:
```shell
screencapture {{path/to/file.png}}
```
#### Take a screenshot including the mouse cursor:
```shell
screencapture -C {{path/to/file.png}}
```
#### Take a screenshot and open it in Preview, instead of saving:
```shell
screencapture -P
```
#### Take a screenshot of a selected rectangular area:
```shell
screencapture -i {{path/to/file.png}}
```
#### Take a screenshot after a delay:
```shell
screencapture -T {{seconds}} {{path/to/file.png}}
```
#### Make a screen recording and save it to a file:
```shell
screencapture -v {{path/to/file.mp4}}
```
{% endraw %}