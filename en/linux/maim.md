---
layout: default
title: "maim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="maim">
  <a href="/en/linux/maim.html">maim</a> <a href="#maim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Screenshot utility.
> More information: <https://github.com/naelstrof/maim>.

#### Capture a screenshot and save it to the given path:
```shell
maim {{path/to/screenshot.png}}
```
#### Capture a screenshot of the selected region:
```shell
maim --select {{path/to/screenshot.png}}
```
#### Capture a screenshot of the selected region and save it in the clipboard (requires `xclip`):
```shell
maim --select | xclip -selection clipboard -target image/png
```
#### Capture a screenshot of the current active window (requires `xdotool`):
```shell
maim --window $(xdotool getactivewindow) {{path/to/screenshot.png}}
```
{% endraw %}