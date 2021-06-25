---
layout: default
title: "colorpicker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="colorpicker">
  <a href="/en/common/colorpicker.html">colorpicker</a> <a href="#colorpicker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A minimalist X11 colorpicker.
> Any mouse gesture except left click will exit the program.
> More information: <https://github.com/ym1234/colorpicker>.

#### Launch colorpicker and print the hexadecimal and RGB value of each clicked pixel to stdout:
```shell
colorpicker
```
#### Only print the color of one clicked pixel and then exit:
```shell
colorpicker --one-shot
```
#### Print the color of each clicked pixel and quit when a key is pressed:
```shell
colorpicker --quit-on-keypress
```
#### Only print the RGB value:
```shell
colorpicker --rgb
```
#### Only print the hexadecimal value:
```shell
colorpicker --hex
```
{% endraw %}