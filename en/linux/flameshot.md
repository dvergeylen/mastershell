---
layout: default
title: "flameshot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flameshot">
  <a href="/en/linux/flameshot.html">flameshot</a> <a href="#flameshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Screenshot utility with a gui interface.
> Supports basic image editing, such as text, shapes, colors, and imgur.
> More information: <https://flameshot.js.org>.

#### Launch flameshot in gui mode:
```shell
flameshot launcher
```
#### Take a screenshot by clicking and dragging:
```shell
flameshot gui
```
#### Take a full screen screenshot:
```shell
flameshot full
```
#### Set the save path to write screenshots to:
```shell
flameshot full --path {{path/to/directory}}
```
#### Delay the screenshot for N milliseconds and output to clipboard:
```shell
flameshot full --delay {{2000}} --clipboard
```
{% endraw %}