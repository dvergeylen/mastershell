---
layout: default
title: "light"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="light">
  <a href="/en/linux/light.html">light</a> <a href="#light"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI to control the backlight of your screen.

#### Get the current backlight value in percent:
```shell
light
```
#### Set the backlight value to 50 percent:
```shell
light -S {{50}}
```
#### Reduce 20 percent from the current backlight value:
```shell
light -U {{20}}
```
#### Add 20 percent to the current backlight value:
```shell
light -A {{20}}
```
{% endraw %}