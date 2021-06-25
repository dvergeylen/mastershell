---
layout: default
title: "xterm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xterm">
  <a href="/en/linux/xterm.html">xterm</a> <a href="#xterm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A terminal emulator for the X Window System.

#### Open the terminal with a title of `Example`:
```shell
xterm -T {{Example}}
```
#### Open the terminal in fullscreen mode:
```shell
xterm -fullscreen
```
#### Open the terminal with a dark blue background and yellow foreground (font color):
```shell
xterm -bg {{darkblue}} -fg {{yellow}}
```
#### Open the terminal with 100 characters per line and 35 lines, in screen position x=200px, y=20px:
```shell
xterm -geometry {{100}}x{{35}}+{{200}}+{{20}}
```
#### Open the terminal using a Serif font and a font size equal to 20:
```shell
xterm -fa {{'Serif'}} -fs {{20}}
```
{% endraw %}