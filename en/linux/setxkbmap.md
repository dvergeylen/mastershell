---
layout: default
title: "setxkbmap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="setxkbmap">
  <a href="/en/linux/setxkbmap.html">setxkbmap</a> <a href="#setxkbmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the keyboard using the X Keyboard Extension.

#### Set the keyboard in French AZERTY:
```shell
setxkbmap {{fr}}
```
#### Set multiple keyboard layouts, their variants and switching option:
```shell
setxkbmap -layout {{us,de}} -variant {{,qwerty}} -option {{'grp:alt_caps_toggle'}}
```
#### Get help:
```shell
setxkbmap -help
```
#### List all layouts:
```shell
localectl list-x11-keymap-layouts
```
#### List variants for the layout:
```shell
localectl list-x11-keymap-variants {{de}}
```
#### List available switching options:
```shell
localectl list-x11-keymap-options | grep grp:
```
{% endraw %}