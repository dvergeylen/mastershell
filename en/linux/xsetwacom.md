---
layout: default
title: "xsetwacom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xsetwacom">
  <a href="/en/linux/xsetwacom.html">xsetwacom</a> <a href="#xsetwacom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to change settings for Wacom pen tablets at runtime.

#### List all the available wacom devices. The device name is in the first column:
```shell
xsetwacom list
```
#### Set Wacom area to specific screen. Get name of the screen with `xrandr`:
```shell
xsetwacom set "{{device_name}}" MapToOutput {{screen}}
```
#### Set mode to relative (like a mouse) or absolute (like a pen) mode:
```shell
xsetwacom set "{{device_name}}" Mode "{{Relative|Absolute}}"
```
#### Rotate the input (useful for tablet-PC when rotating screen) by 0|90|180|270 degrees from "natural" rotation:
```shell
xsetwacom set "{{device_name}}" Rotate {{none|half|cw|ccw}}
```
#### Set button to only work when the tip of the pen is touching the tablet:
```shell
xsetwacom set "{{device_name}}" TabletPCButton "on"
```
{% endraw %}