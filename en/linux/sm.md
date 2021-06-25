---
layout: default
title: "sm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sm">
  <a href="/en/linux/sm.html">sm</a> <a href="#sm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays a short message fullscreen.
> More information: <https://github.com/nomeata/screen-message>.

#### Display a message in full-screen:
```shell
sm "{{Hello World!}}"
```
#### Display a message with inverted colors:
```shell
sm -i "{{Hello World!}}"
```
#### Display a message with a custom foreground color:
```shell
sm -f {{blue}} "{{Hello World!}}"
```
#### Display a message with a custom background color:
```shell
sm -b {{#008888}} "{{Hello World!}}"
```
#### Display a message rotated 3 times (in steps of 90 degrees, counterclockwise):
```shell
sm -r {{3}} "{{Hello World!}}"
```
#### Display a message using the output from another command:
```shell
{{echo "Hello World!"}} | sm -
```
{% endraw %}