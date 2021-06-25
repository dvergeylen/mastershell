---
layout: default
title: "xdotool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xdotool">
  <a href="/en/linux/xdotool.html">xdotool</a> <a href="#xdotool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line automation for X11.

#### Retrieve the X-Windows window ID of the running Firefox window(s):
```shell
xdotool search --onlyvisible --name {{firefox}}
```
#### Click the right mouse button:
```shell
xdotool click {{3}}
```
#### Get the id of the currently active window:
```shell
xdotool getactivewindow
```
#### Focus on the window with id of 12345:
```shell
xdotool windowfocus --sync {{12345}}
```
#### Type a message, with a 500ms delay for each letter:
```shell
xdotool type --delay {{500}} "Hello world"
```
#### Press the enter key:
```shell
xdotool key {{KP_Enter}}
```
{% endraw %}