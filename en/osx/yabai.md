---
layout: default
title: "yabai"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yabai">
  <a href="/en/osx/yabai.html">yabai</a> <a href="#yabai"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tiling window manager for macOS based on binary space partitioning.
> More information: <https://github.com/koekeishiya/yabai>.

#### Set the layout to bsp:
```shell
yabai -m config layout {{bsp}}
```
#### Set the window gap to 10pt:
```shell
yabai -m config window_gap {{10}}
```
#### Enable opacity:
```shell
yabai -m config window_opacity on
```
#### Disable window shadow:
```shell
yabai -m config window_shadow off
```
#### Enable status bar:
```shell
yabai -m config status_bar on
```
{% endraw %}