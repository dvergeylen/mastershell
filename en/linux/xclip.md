---
layout: default
title: "xclip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xclip">
  <a href="/en/linux/xclip.html">xclip</a> <a href="#xclip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> X11 clipboard manipulation tool, similar to `xsel`.
> Handles the X primary and secondary selections, plus the system clipboard (`Ctrl + C`/`Ctrl + V`).

#### Copy the output from a command to the X11 primary selection area (clipboard):
```shell
echo 123 | xclip
```
#### Copy the output from a command to a given X11 selection area:
```shell
echo 123 | xclip -selection {{primary|secondary|clipboard}}
```
#### Copy the output from a command to the system clipboard, using short notation:
```shell
echo 123 | xclip -sel clip
```
#### Copy the contents of a file into the system clipboard:
```shell
xclip -sel clip {{input_file.txt}}
```
#### Copy the contents of a PNG image into the system clipboard (can be pasted in other programs correctly):
```shell
xclip -sel clip -t image/png {{input_file.png}}
```
#### Copy the user input in the console into the system clipboard:
```shell
xclip -i
```
#### Paste the contents of the X11 primary selection area to the console:
```shell
xclip -o
```
#### Paste the contents of the system clipboard to the console:
```shell
xclip -o -sel clip
```
{% endraw %}