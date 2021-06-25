---
layout: default
title: "pastel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pastel">
  <a href="/en/common/pastel.html">pastel</a> <a href="#pastel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate, analyze, convert and manipulate colors.
> More information: <https://github.com/sharkdp/pastel>.

#### Convert colors from one format to another. Here from RGB to HSL:
```shell
pastel format {{hsl}} {{ff8000}}
```
#### Show and analyze colors on the terminal:
```shell
pastel color "{{rgb(255,50,127)}}"
```
#### Pick a color from somewhere on the screen:
```shell
pastel pick
```
#### Generate a set of N visually distinct colors:
```shell
pastel distinct {{8}}
```
#### Get a list of all X11 / CSS color names:
```shell
pastel list
```
{% endraw %}