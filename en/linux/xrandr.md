---
layout: default
title: "xrandr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xrandr">
  <a href="/en/linux/xrandr.html">xrandr</a> <a href="#xrandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the size, orientation and/or reflection of the outputs for a screen.

#### Display the current state of the system (known screens, resolutions, ...):
```shell
xrandr --query
```
#### Disable disconnected outputs and enable connected ones with default settings:
```shell
xrandr --auto
```
#### Change the resolution and update frequency of DisplayPort 1 to 1920x1080, 60Hz:
```shell
xrandr --output {{DP1}} --mode {{1920x1080}} --rate {{60}}
```
#### Set the resolution of HDMI2 to 1280x1024 and put it on the right of DP1:
```shell
xrandr --output {{HDMI2}} --mode {{1280x1024}} --right-of {{DP1}}
```
#### Disable the VGA1 output:
```shell
xrandr --output {{VGA1}} --off
```
#### Set brightness for LVDS1 to 50%:
```shell
xrandr --output {{LVDS1}} --brightness {{0.5}}
```
#### See display hardware information:
```shell
xrandr -q
```
{% endraw %}