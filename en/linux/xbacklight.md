---
layout: default
title: "xbacklight"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xbacklight">
  <a href="/en/linux/xbacklight.html">xbacklight</a> <a href="#xbacklight"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to adjust backlight brightness using the RandR extension.
> More information: <https://gitlab.freedesktop.org/xorg/app/xbacklight>.

#### Get the current screen brightness as a percentage:
```shell
xbacklight
```
#### Set the screen brightness to 40%:
```shell
xbacklight -set {{40}}
```
#### Increase current brightness by 25%:
```shell
xbacklight -inc {{25}}
```
#### Decrease current brightness by 75%:
```shell
xbacklight -dec {{75}}
```
#### Increase backlight to 100%, over 60 seconds (value given in ms), using 60 steps:
```shell
xbacklight -set {{100}} -time {{60000}} -steps {{60}}
```
{% endraw %}