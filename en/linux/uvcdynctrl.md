---
layout: default
title: "uvcdynctrl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uvcdynctrl">
  <a href="/en/linux/uvcdynctrl.html">uvcdynctrl</a> <a href="#uvcdynctrl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A libwebcam command-line tool to manage dynamic controls in uvcvideo.

#### List all available cameras:
```shell
uvcdynctrl -l
```
#### Specify the device to use (defaults to `video0`):
```shell
uvcdynctrl -d {{device_name}}
```
#### List available controls:
```shell
uvcdynctrl -c
```
#### Set a new control value (for negative values, add -- before {{-value}}):
```shell
uvcdynctrl -s {{control_name}} {{value}}
```
#### Get the current control value:
```shell
uvcdynctrl -g {{control_name}}
```
#### Save the state of the current controls to a file:
```shell
uvcdynctrl -W {{filename}}
```
#### Load the state of the controls from a file:
```shell
uvcdynctrl -L {{filename}}
```
{% endraw %}